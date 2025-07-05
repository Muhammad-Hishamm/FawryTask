# FawryTask E-Commerce System

## Overview

FawryTask is a simple e-commerce system implemented in C# (.NET 8) that demonstrates core shopping cart functionality, product management, and shipping fee calculation. The project models products, shippable products, customers, and a cart, and provides logic for adding/removing items, checking out, and calculating shipping costs.

## Features

- **Product Management:**  
  Supports both regular and shippable products, each with properties like name, price, quantity, and (optionally) expiration date.

- **Shopping Cart:**  
  Add or remove products and shippable products to/from a cart. The cart keeps track of quantities and supports price calculation.

- **Shipping Services:**  
  Calculates total shipping weight and fees for shippable products in the cart.

- **Customer Model:**  
  Represents customers with an ID and balance, supporting checkout operations.

## Project Structure

- `Product.cs` – Base class for all products.
- `ShippableProduct.cs` – Inherits from `Product`, adds weight property.
- `Cart.cs` – Manages products and shippable products in a shopping cart.
- `Customer.cs` – Represents a customer.
- `ShippingServices.cs` – Calculates shipping weight and fees.
- `IShippingServices.cs` – Interface for shipping services.
- `Program.cs` – Entry point with example usage and test cases.

## Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- Visual Studio 2022 or later

### Build and Run

1. Clone the repository.
2. Open the solution in Visual Studio.
3. Build the solution.
4. Run the project.  
   The console will display test outputs for the e-commerce system.

## Example Usage

The `Program.cs` file demonstrates:

- Creating products and shippable products.
- Creating customers.
- Adding items to a cart.
- Checking out and calculating shipping fees.

## Shipping Fee Calculation

Shipping fees are calculated based on the total weight (in kilograms) of shippable products in the cart, using a fixed rate per kilogram.


