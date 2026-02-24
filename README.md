# Case Study 1
Grocery-Billing-System_PalakPandey_202501100700101_B
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
