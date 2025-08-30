
Fintech Wallet API Documentation

This project is a sample API documentation for a digital wallet system.
I created it using Postman to practice how fintech companies design and document APIs.

The goal is to show how users can:

Create and manage wallets

Send and receive payments

Check balances

View transaction history

Why I built this

As a junior API technical writer, I wanted to practice writing clear, simple API docs that any developer (or non-developer) can understand.
This repo shows how I approach:

Organizing endpoints

Writing simple explanations

Adding example requests and responses

Endpoints Overview
1. Wallets

Create a wallet → POST /wallets

Get wallet details → GET /wallets/{id}

Check balance → GET /wallets/{id}/balance

2. Transactions

Send money → POST /transactions/send

Receive money → POST /transactions/receive

Transaction history → GET /transactions

3. Users

Register user → POST /users/register

Login → POST /users/login

Get user profile → GET /users/{id}

Example Request (Postman)

Send Money

http
POST /transactions/send

Body (JSON)

{
  "from_wallet": "wallet_123",
  "to_wallet": "wallet_456",
  "amount": 100,
  "currency": "USD"
}

Response

{
  "status": "success",
  "transaction_id": "txn_001",
  "message": "Transfer completed"
}

What’s Inside

This is the postman link.

https://documenter.getpostman.com/view/47844697/2sB3HevjFC

Fintech-Wallet-API.postman_collection.json → Import into Postman to test endpoints.

README.md → You are reading it

My Learnings

How to structure API endpoints clearly

How to explain requests/responses step by step

The importance of examples for beginners

This is a practice project for learning API documentation. Not a real payment system.
