```python
list = ["10000","5000","1000","500","100","50","10","1"]
another_list =[]
def namename(num, money_to_change,what_change_by):
    if money_to_change % num == 0:
        final_exchange = money_to_change / num
        for i in list:
            if what_change_by == i:
                print(final_exchange)
                another_list.append(final_exchange)
    else:
        final_exchange = "Put more money"
        print(final_exchange)
    return final_exchange



money_to_change = int(input("how much do you want to exchange?(put number here)"))
what_change_by = input("10000,5000,1000,500,100,50,10,1")

for n in list:
    if what_change_by == n:
        num = int(n)
        # print("cant change")
        namename(num, money_to_change, what_change_by)
        print(another_list[-1])
    # else:
    #     print("no")
```
