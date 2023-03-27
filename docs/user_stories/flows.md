# User stories' flows

This file documents the basic flows for the user stories. The objective here is to create a initial idea of how the user stories will work in real life. With that in hands it'll be easier to build prototypes.

---

## 01 As consumer, I want to visit virtual stores to see what the producer is selling.

The consumer can be authenticated or not.

1. The consumer access the "virtual stores" page, where is shown the stores.
2. The consumer clicks on a virtual store.
3. The system shows the virtual store's basic data (producer's name, location, number of sales, since when he's registered at OrganicLocker) and it's available products.

## 02 As consumer, I want to purchase products with my credit card.

The consumer must be authenticated.

1. At a virtual store page, the consumer adds products to the basket.
2. The consumer then clicks on "proceed to checkout".
3. The system shows the list of products in the basket.
4. The consumer can increase/decrease the number of a specific product or exclude it.
5. The consumer must set the delivery/collection location for each producer that he's buying from.
6. The consumer then clicks on "proceed to payment".
7. The system shows a form.
8. The consumer inputs credit card data.
9. The systems confirms the payment and redirects the consumer to "My Purchases" page.

## 07 As consumer/producer, I want to register myself at OrganicLocker.

The consumer/producer must not be authenticated.

1. At any page, the user clicks on "register".
2. The system shows the register form.
3. The user inputs his data (name, e-mail, password, location: city and neighborhood) and clicks on "register.
4. The system confirms the registration and redirects the user to login page.

## 08 As producer, I want to register my products.

The producer must be authenticated.
The producer must have created a virtual store.

1. The producer goes to "My Products" page.
2. The system shows a list of all producer's products.
3. The producer clicks on "add product".
4. The system shows a form for product registration.
5. The producer inputs the product data (product name, photo, product type, description, quantity available and expiration date) and clicks on "register product".
6. The system confirms the product registration and redirects the user to "My Products".

## 09 As producer, I want to make my products available or unavailable to sell.

The producer must be authenticated.
The producer must have created a virtual store.

1. The producer goes to "My Products" page.
2. The system shows a list of all producer's products.
- To make a product unavaible, the producer clicks on the respective icon on the product card.
- To make a product available, the producer clicks on the respecitve icon oh the product card.
  4. The system shows an input field where the producer inputs the quantity available and expiration date.
  5. The producer clicks on "save" button.
  6. The system confirms the action and refreshes the page.

## 10 As producer, I want to confirm/cancel the purchase of a product.

The producer must be authenticated.
The producer must have created a virtual store.
A consumer must have purchased a product.

1. The producer goes to the tab "Pending confirmation" in "My sales" page.
2. The system shows all pending confirmation sales for that producer.
3. The producer can:
    1. click on "Confirm all" to confirm the sale as whole;
    2. click on "Cancel all" to cancel the sale as whole;
    3. confirm and cancel items individually.
4. The system confirms the action and refreshes the page.
5. The systens send an e-mail to the consumer.

## 11 As producer, I want to register the delivery of the products.

The producer must be authenticated.
The producer must have created a virtual store.
A consumer must have purchased a product.
The producer must have confirmed a sale.

1. The producer goes to the tab "Confirmed" in "My sales" page.
2. The system shows all confirmed sales for that producer.
3. The producer clicks on "Confirm delivery" on the specific sale card.
4. The system shows a QR code.
5. The producer authenticates the QR code on the reader at the locker.
6. The system confirms the delivery and refreshes the page.

## 12 As consumer, I want to register the collection of the products I purchased.

The consumer must be authenticated.
The consumer must have a deliver-confirmed purchased.

1. The consumer goes to the tab "Delivered" in "My purchases" page.
2. The system shows all delivered purchases from that consumer.
3. The consumer clicks on "Confirm collection" on the specific purchase card.
4. The system shows a QR code.
5. The consumer authenticates the QR code on the reader at the locker.
6. The system shows a question asking if the consumer got the products.
7. The consumer answers positively.
8. The systems confirms the action and refreshes the page.

If the consumer does not answer the step 7 positively, the system must show an error and refreshes the page.

## 21 As producer, I want to create my virtual store.

The producer must be authenticated.

1. The producer goes to "My virtual store" page.
2. The system shows a page only saying that the user has not yet created a virtual store.
3. The producer clicks on "Create virtual store".
4. The system shows the virtual store creation form.
5. The producer inputs the name of its virtual store, the days of the week it delivers its products and the delivery/collection locations, and uploads the organic producer certification.
6. The system confirms the registration and redirects the producer to "My Products" page.
