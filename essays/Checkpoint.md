---
layout: essay
type: essay
title: "Checkpoint Assignment #3"
# All dates must be YYYY-MM-DD format!
date: 2022-12-30
published: true
labels:
  - Checkpoint
  - Assignment 3
---

## Checkpoint Assignment #3

### 1.  Show what each page will look like. The pages do not have to be "functional" but the design should be clear.

![gabriel'sWalletStore](https://i.imgur.com/mllJiNN.png)
 
### 2.  Describe your design for your site's shopping cart. That is, will it be a separate page that that the user can view and edit, or will it be integrated into the product pages? If so, describe in detail how this will work on your site. Provide several examples of using the cart.

My plan is to integrate the shopping cart into the home or product pages so users can view their carts without leaving their current page. It will store the user's purchase information based on the data within the user's session. An 'add to cart' button will appear when a user selects a quantity from a product, and once clicked, it will create a new key-value pair in their session. Users may add to their cart at any time, but to proceed to the invoice, they must be logged in. Otherwise, they are redirected to the login page. The user iS able to modify the quantities of items already selected in the shopping cart. Users will be limited to the quantity of inventory available when a entering a quantity.

### 3.  Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, and what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and and their objects) you will use to manage the shopping cart data and how they will be used in a session.

I will implement sessions in Assignment 3 to manage my shopping cart information, such as what products are selected and how many of each product are selected. By holding this information in a session with an array, The following is an example; `request.session.cart[products key] = userQuantities` where userQuantities is the array defined to store quantities input by the user. The user can view and edit this information in the shopping cart. My intention is to write a program that will overwrite the old information with the updated information when editing it.

### 4.  How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?

By using cookies, I plan to make sure that users are logged out after a specified period of time (10 minutes). When a user visits the site, if the cookie stored on their browser does not match a session, they will have to login or register.

### 5.  Upon a successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary)

Cookies and session information will be used to implement the following: When a user successfully logs in, the login button will be replaced by his or her name in the nay bar. That button allows users to edit their accounts or log out. Additionally, the navigation bar will display the number of items in the shopping cart based on cookies and session information.

### 6.  If you are working with partners, how will you split up the work in your team SO that you are working in parallel as effectively as possible? That is, who is doing what and when?

As I do not have a partner, I am unable to respond to this question.

### 7.  How are you approaching Assignment 3 differently than Assignment 2?

There are a number of different elements in this assignment, such as login, different product pages, and the cart. The complexities of these elements prompted me to consider my options carefully before starting the coding process. For Assignment 2, I put myself through a trial and error process, but hopefully, this will change for Assignment 3. It would be very beneficial for me if was able to thoroughly think through them as to what syntax to use and how everything could be organized.
  
