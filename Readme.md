# RapydPay Payment System

# Overview

### This is a Payment Platorm that supports sending and transfering of payments. This application uses [Rapyd](https://www.rapyd.net/) payment APIs to handle payments of the user.

# Prerequisite

### [Rapyd Account](https://www.rapyd.net/)

### [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register)

### [Node.js](https://nodejs.org/en/download/)

# Installation Guidelines

## STEP 1

```sh
  git clone from file directory
```

## STEP 2

- ### Note - Run this command in the root directory as well as in the frontend directory.
- ### cd frontend

```sh
   npm install
```

## STEP 3

- ### After downloading all the Frontend Dependencies.
- ### Run this command in the frontend directory

```sh
   npm run build
```

## STEP 4

- #### [Get Your Rapyd Access key and Secret key from Rapyd client portal](https://dashboard.rapyd.net/developers)
- #### Note - Create .env file in the root directory with following variables.

  ```sh
  PORT = 5000
  ACCESS_KEY =
  SECRET_KEY =
  MONGO_URI =
  ```

## STEP 5

### Run this in the root directory

```sh
 npm start
```

## STEP 6

- ### The project will be served in this port if you have done all the above steps correctly. 🥇

```sh
http://localhost:5000/
```

## Test cards

- ### Note - Initially the total balance of the wallets will be zero. So you can create a customer with the wallet id and rapyd test cards to fund your wallets.
- ### [Here's a link to Rapyd Test cards for payments and transactions](https://docs.rapyd.net/build-with-rapyd/reference/testing-for-payments-api)

# Features

## 1. Create Wallet Features

- ### [User can fill up their credentials and create wallet which generates a unique wallet ID.](https://user-images.githubusercontent.com/67522406/123187564-0baead00-d4b8-11eb-94c8-9d4cce6f294b.png)

- ### [All the Wallet Details with the unique wallet ID shows up in the wallet Section.](https://user-images.githubusercontent.com/67522406/123187556-07828f80-d4b8-11eb-88e4-0dc331efa43d.png)

- ### [Money Transactions can be done between wallets with Sender's WalletID , Amount (in USD) and Recievers WalletID.](https://user-images.githubusercontent.com/67522406/123187599-19fcc900-d4b8-11eb-92fb-61e066a6fe71.png)

- ### [The total balance of both the wallets gets updated after successfull Transaction between wallets.](https://user-images.githubusercontent.com/67522406/123187556-07828f80-d4b8-11eb-88e4-0dc331efa43d.png)

## 2. Accesing Transactions of a Wallet

- ### [Transactions of a particular wallet can be viewed by clicking on the view transaction button on each wallet card.](https://user-images.githubusercontent.com/67522406/123187610-1ec17d00-d4b8-11eb-8025-baf86c48bbcc.png)
- ### [Transaction detail conatins the transacion ID , Amount Debited/credited, Date and wallet id of the wallet to which the amount is paid or recieved.](https://user-images.githubusercontent.com/67522406/123187610-1ec17d00-d4b8-11eb-8025-baf86c48bbcc.png)

- ### [If the amount is credited to the wallet it shows in green and if the amount is debited it shows in Red.](https://user-images.githubusercontent.com/67522406/123187610-1ec17d00-d4b8-11eb-8025-baf86c48bbcc.png)

### Important Points To remember for creating wallet

- #### You can create only one wallet with single Email-ID or Phone Number.
- #### The number should be in E.164 format (Ex- +918247564782)

## 3. Creating customer with a wallet

- ### [Customer can be created for each wallet with a default Visa card number and details of the customer.](https://user-images.githubusercontent.com/67522406/123187664-3436a700-d4b8-11eb-83cb-3d575d62820e.png)

- ### [Customer Section will contain the information of all the customers. Each customer will have their own customeID and walletd id associated with it.](https://user-images.githubusercontent.com/67522406/123187650-30a32000-d4b8-11eb-93ce-9e3c937dac53.png)

### Important Points To remember for creating customer

- #### You can create only one customer using one wallet but you can fund multiple wallets using a single customer.

## 4 . Accessing payments of a Customer

- ### [Customers can pay to any wallets and the amount will be debited from the associated default visa card of the cutomer from which it was initially created. ](https://user-images.githubusercontent.com/67522406/123187670-3862c480-d4b8-11eb-80fe-1e4d5f0ac115.png)

- ### [The amount paid by the customer is added to the wallet and the balance gets updated in the total balance of the ewallet.](https://user-images.githubusercontent.com/67522406/123187556-07828f80-d4b8-11eb-88e4-0dc331efa43d.png)

- ### [The payment details of a particular customer conatins the Pament Id and the wallet id to which the amount was paid.](https://user-images.githubusercontent.com/67522406/123187677-3b5db500-d4b8-11eb-9dfd-cfe4483c31b5.png)

- ### [If the amount is paid from the customers associated wallet it shows up in green and if it is paid to another wallet it shows in green.](https://user-images.githubusercontent.com/67522406/123187677-3b5db500-d4b8-11eb-9dfd-cfe4483c31b5.png)

## 5 . Checkout

- ### [Products can be buyed from the products section using rapyd hosted checkout ]


