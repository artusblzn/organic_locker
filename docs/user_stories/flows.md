# User stories' flows

This file documents the basic flows for the user stories. The objective here is to create a initial idea of how the user stories will work in real life. With that in hands it'll be easier to build prototypes.

---

## 01 As consumer, I want to visit virtual stores to see what the producer is selling.

The consumer can be authenticated or not.

1. The consumer access the "Producers" page, where is shown the stores.
2. The consumer clicks on a virtual store.
3. The system shows the virtual store's basic data (producer's name, location, since when he's registered at OrganicLocker, the day it delivers the products and the delivery lockers it uses) and it's available products.

## 02 As consumer, I want to purchase products with my credit card.

The consumer must be authenticated.

1. At a virtual store page, the consumer selects the quantity of the products he wants to purchase.
2. The consumer then clicks on "Proceed to Checkout".
3. The system shows the list of delivery lockers.
4. The consumer selects a delivery locker.
5. The system shows a form.
6. The consumer inputs credit card data and confirms it.
7. The system shows the order details.
8. The consumer clicks on confirm.
9. The system confirms the payment and redirects the consumer to "My Orders" page.

## 07 As consumer/producer, I want to register myself at OrganicLocker.

The consumer/producer must not be authenticated.

1. At any page, the user clicks on "register".
2. The system shows the register form.
3. The user inputs his data (name, e-mail, password, location: city) and clicks on "register".
4. The system confirms the registration and redirects the user to login page.

## 08 As producer, I want to register my products.

The producer must be authenticated.
The producer must have created a virtual store.

1. The producer goes to "My Products" page.
2. The system shows a list of all producer's products.
3. The producer clicks on "Add product".
4. The system shows a form for product registration.
5. The producer inputs the product data (product name, product type, description, quantity available and expiration date) and clicks on "register product".
6. The system confirms the product registration and redirects the user to "My Products".

## 09 As producer, I want to make my products available or unavailable to sell.

The producer must be authenticated.
The producer must have created a virtual store.

1. The producer goes to "My Products" page.
2. The system shows a list of all producer's products.
- To make a product unavaible, the producer clicks on the respective icon on the product card.
- To make a product available, the producer clicks on the respecitve icon oh the product card.
3. The system refreshes the product card.

## 10 As producer, I want to confirm/cancel an order.

The producer must be authenticated.
The producer must have created a virtual store.
A consumer must have purchased a product.

1. The producer goes to the tab "Pending confirmation" in "Orders Received" page.
2. The system shows all pending confirmation sales for that producer.
3. The producer can:
    1. click on "Confirm" to confirm the sale as whole;
    2. click on "Cancel" to cancel the sale as whole;
4. The system confirms the action and refreshes the page.
5. The system sends an e-mail to the consumer.

## 11 As producer, I want to register the delivery of the products.

The producer must be authenticated.
The producer must have created a virtual store.
A consumer must have purchased a product.
The producer must have confirmed a sale.

1. The producer goes to the tab "Confirmed" in "Orders Received" page.
2. The system shows all confirmed orders for that producer.
3. The producer clicks on "Confirm delivery" icon on the specific sale card.
4. The system shows a QR code.
5. The producer authenticates the QR code on the reader at the locker.
6. The system confirms the delivery and refreshes the page.

## 12 As consumer, I want to register the collection of an order I made.

The consumer must be authenticated.
The consumer must have a deliver-confirmed purchase.

1. The consumer goes to the tab "Delivered" in "My Orders" page.
2. The system shows all delivered purchases from that consumer.
3. The consumer clicks on "Confirm collection" on the specific purchase card.
4. The system shows a QR code.
5. The consumer authenticates the QR code on the reader at the locker.
6. The system shows a question asking if the consumer got the products.
7. The consumer answers positively.
8. The system confirms the action and refreshes the page.

If the consumer does not answer the step 7 positively, the system must show an error and refreshes the page.

## 21 As producer, I want to create my virtual store.

The producer must be authenticated.

1. The producer goes to "My virtual store" page.
2. The system shows a page only saying that the user has not yet created a virtual store.
3. The producer clicks on "Create virtual store".
4. The system shows the virtual store creation form.
5. The producer inputs the name of its virtual store, the days of the week it delivers its products and the delivery/collection locations, and uploads the organic producer certification.
6. The system confirms the registration and redirects the producer to "My Products" page.

## 24 As producer, I want to edit my products.

The producer must be authenticated.
The producer must have a product registered.
This action can only be taken if the product had not been bought yet.

1. The producer goes to "My Products" page.
2. The system shows a list of all producer's products.
3. The producer clicks the "Edit" icon on product card.
4. The system shows a pre-filled form.
5. The producer edits the forms and confirms.
6. The system goes to "My Products".
