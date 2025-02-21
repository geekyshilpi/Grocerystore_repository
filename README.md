#By using user input approach.....
prices=[]
i=int(input("No. of prices u want to enter : "))
cnt=0
while(cnt<i):
  a=int(input("Enter the price of item : "))
  b=int(input("Discount offered : "))
  prices.append(float(a*((100-b)/100)))
  cnt+=1
sum=0
z=0
while(z<i):
  sum=sum+prices[z]
  z+=1
print("Total Discounted Prices : ",sum)
print("Total Price after GST : ",float(sum+sum*0.18))
