# Book-Record-Management

This is a book record management API Backend for the management of records and books

# API Documentation link

https://documenter.getpostman.com/view/22926115/2s8Ysp1vFZ

# Routes and Endpoints

## /users

POST: Create a new user ✅
GET: Get all list of users ✅

## /usres/{id}

GET: Get a user by id ✅
PUT: Update a user by id ✅
DELETE: Delete a user by id (check if he/she still has an issued book) (is there any fine to be paid) ✅

## /users/subcription-details/{id}

GET: Get user subcription details ✅

1. Date of subcription
2. Valid till
3. Fine if any 

## /books

GET: Get all books ✅
POST: Create/Add a new book ✅

## /books/{id}

GET: get a book by id ✅
PUT: update a book by id ✅

## /books/issued/by-user

GET: Get all issued books ✅

## /books/issued/withFine

GET: get all issued books with fine

# Subcription Type

Basic (3 months)
Standard (6 months)
Premium (12 months)

NOTE: Dates will be in format mm/dd/yyyy


If the subscription date is 01/08/22
and Subscription type is Standard 
the valid till date will be 01/02/23


If he has an issued book and the issued book is to be returned at 01/01/23
If he missed the date of return, then he gts a fine of Rs. 100./


If he has an issued book and the issued book is to be returned at 01/01/23
If he missed the date of return, and his subscription also expires, then he will get a fine of Rs 200./