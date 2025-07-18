# 🚗 Car Rental Management System (Python)

A simple object-oriented Python program to simulate a car rental system. The system allows customers to rent and return cars while managing availability, rental records, and tracking rental fees.

## 📋 Features

* Add and manage Cars with availability status
* Register and manage Customers
* Enable Renting and Returning of cars
* Maintain Rental Records including rental ID, customer, car, and rental fee
* Display customer's rented cars and rental information

## 🧱 Classes Overview

### Car

Represents a car in the rental system.

Attributes:

* car_id
* make
* model
* year
* available

Methods:

* rent() – Marks car as rented
* return_car() – Marks car as available again

---

### Customer

Represents a customer who can rent one or more cars.

Attributes:

* customer_id
* name
* rented_cars (list of rented Car objects)

Methods:

* rent_car(car) – Rents a car if available
* return_car(car) – Returns a rented car

---

### Rental

Represents a rental record between a customer and a car.

Attributes:

* rental_id
* customer
* car
* rental_fee

---

## 🚀 Usage

python
# Initialize cars and customers
cars = [...]
customers = [...]

# Rent cars
customers[0].rent_car(cars[0])

# Return cars
customers[0].return_car(cars[0])

# Create rental records
rentals = [
    Rental("R001", customers[0], cars[0], 5000.0)
]

# Display rental info
for rental in rentals:
    print(f"Rental ID: {rental.rental_id}, Customer: {rental.customer.name}, Car: {rental.car.make}")


## 📦 Requirements

This project is implemented in pure Python and does not require any external libraries.

Tested on:

* Python 3.8+
* Python 3.10

## 🛠 Installation

1. Clone the repository:

   bash
   git clone https://github.com/yourusername/car-rental-system.git
   cd car-rental-system
   

2. Run the script:

   bash
   python car_rental.py
   

## ✅ Output Example

plaintext
Aarya Meshram's Rented Cars: ['Toyota']
Monika Doble's Rented Cars: ['Honda']
...

Aarya Meshram's Updated Rented Cars: []
Monika Doble's Updated Rented Cars: ['Honda']
...

Rental ID: R001, Customer: Aarya Meshram, Car: Toyota, Rental Fee: INR 5000.0
...

## 🙌 Acknowledgments

* Inspired by real-world car rental processes.
* Built for learning and demonstration purposes.

---

Let me know if you'd like a logo or markdown badges added!

Name:Monika Doble
Contact:9890885432
Email:monikadoble7@gmail.com
