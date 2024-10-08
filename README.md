# assignment-9
#Q
# To find BOD at 7th day 25C
# To find Decay Coefficient at 25C
K= float(input("Decay Coefficient:"))
T= float(input("Temperature of 3rd day BOD:"))
TI=float(input("Temperature of 7th day BOD:"))
K2 = (K*(1.047**(TI-T)))
print ("The value ofK2 is:", K2)
# To find Ultimate BOD
e=2.718
print ("The value ofe is:", e)
Bl = float(input("BOD at 3rd day 20c:"))
t = float(input("time in days for finding B1:"))
E = (1 - 2.71828 ** (-0.23 * t))
print ("The value of E is:", E)
BI = 10 * E
print ("The value of 10 is:", 10)
# To find BOD at 7th day 25C
B2 = float(input("BoD at 7rd day 25c:"))
t1 =float(input("time in days for findinfB2:"))
El =(1-e**(-0.289*t1))
print ("The value ofEl is:", El)
B2 = (10*El)
print ("The value of B2 is:", B2)

#Q.
#Determination if density of sludge removed from aeration tank
M= float(input("Enter the value of initial mass :"))
S=float(input("Enter the value ofsolid containing sludge in percentage:"))
Gs= float(input("Enterthe value of Specific gravity ofsludge solid:"))
Rho_W= float(input("Enter the value of density of water:"))
Ws= ((S/M)*100)
m=M- Ws
print("the value ofmass of water:",m)
print("The value of Solid Content in sludge :",Ws)
Vw =m/Rho_W
print ("The Value of Volume:",Vw)
Rho_S =Gs * Rho_W
print("The value ofDensity of solid content in sludge:", Rho_S)
Vs=(Ws/(Gs*Rho_S ))
print("The value of volume of solid content in sludge:", Vs)
Vt= Vw + Vs
print("The value of total volume of solid content in sludge:", Vt)
Rho_SL= M/ Vt
print("The value of Density of sludge removed from aeration:", Rho_SL)
