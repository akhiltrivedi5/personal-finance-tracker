# Personal Finance Tracker – Data Model

## Transaction
- id (integer, primary key)
- date (date)
- amount (decimal)
- type (income | expense | investment)
- category_id (foreign key)
- payment_method_id (foreign key)
- description (text)
- created_at (timestamp)
- updated_at (timestamp)

## Category
- id (integer, primary key)
- name (text)
- parent_id (nullable foreign key)

## PaymentMethod
- id (integer, primary key)
- name (text)