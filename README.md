＃-批梯度下降
x = [(2.104),(1.416),(1.534),(0.852)]
y = [460,232,315,178]
J0=0
J1=0
m=len(x)
zero=0.001
alpha=0.01
theta01=1
theta11=1
theta00=100
theta10=100
while(theta00-theta01>zero or theta10-theta11>zero):
    for i in range(m):
        h=theta01+theta11*x[i]
        J0=J0+h-y[i]
        J1=J1+(h-y[i])*x[i]
    theta00=theta01
    theta10=theta11
    theta01=theta01-alpha*J0/m
    theta11=theta11-alpha*J1/m
打印（theta01，theta11）x = [(2.104),(1.416),(1.534),(0.852)]
y = [460,232,315,178]
J0=0
J1=0
m=len(x)
zero=0.001
alpha=0.01
theta01=1
theta11=1
theta00=100
theta10=100
while(theta00-theta01>zero or theta10-theta11>zero):
    for i in range(m):
        h=theta01+theta11*x[i]
        J0=J0+h-y[i]
        J1=J1+(h-y[i])*x[i]
    theta00=theta01
    theta10=theta11
    theta01=theta01-alpha*J0/m
    theta11=theta11-alpha*J1/m
print(theta01,theta11)

＃随机梯度下降
