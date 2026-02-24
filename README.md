PROBLEEM STATEMENT 
A grocery store wants to calculate the total cost of 5 different items purchased by a customer.
Each item can be bought in multiple quantities.

If the total bill exceeds Rs. 100, a 10% discount should be applied.
Finally, display the total amount, discount (if any), and the final payable amount.

Approach
1. User enters the price of 5 items.
2. User enters the quantity for each item.
3. The program calculates the total cost:

CODE
total = 0
items=int(input("Enter number of items: "))
for i in range(1,items+1):
    price = float(input("Enter price: "))
    items_quantity = int(input("Enter quantity: "))
    total = total + (price *items_quantity)
print("Original Total =", total)
if total > 100:
    discount = total * 0.10
else:
    discount = 0
print("Discount =", discount)
final_amount = total - discount
print("Final Amount =", final_amount)

OUTPUT
Enter number of items: 6
Enter price: 100
Enter quantity: 10
Enter price: 200
Enter quantity: 16
Enter price: 800
Enter quantity: 5
Enter price: 50
Enter quantity: 13
Enter price: 25
Enter quantity: 15
Enter price: 85
Enter quantity: 26
Original Total = 11435.0
Discount = 1143.5
Final Amount = 10291.5
