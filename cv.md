# **Rondalev Stanislav**
<img src="Rondalev.JPG" align=left width="200" height="220" alt="Rondalev">
<br>
<br>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; *Contact information:*

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; *1. Email: stanislavrondalev@gmail.com,*\
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; *2. Phone number: +375257466653,*\
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; *3. [http://m.vk.com/id667463426](http://m.vk.com/id667463426).*
<br>
<br>
<br>
<br>
## **Brief information about me**
Mo goal is to find a good job to earn good money. Priority: live peacefully and calmy. I am good at **math and programming**. I like to gain new knowledge in mathematics and programming.
## **Skills**
* Proficiency in the Python programming language
* Some knowledge of mathematics
## **Work experience**
Course projects in mathematics, which used knowledge<br>of mathematics and programming in Python: 
* Cycles in graphs;
* Incomplete differential equations of the second order, their physical applications.

And also Curriculum vitae.
## **Example code**
```
from sympy import symbols, diff
from math import isclose
import matplotlib.pyplot as plt
import numpy as np
def numbers_after_point(n):
	from decimal import Decimal
	n=Decimal(str(n))
	count=0
	while (n%1)!=0:
		n*=10
		count+=1
	return count
x, y, φ=symbols('x y φ')
y=x**3-x-5
xg = np.linspace(-4, 4, 20)
yg = [y.subs(x, i) for i in xg]
plt.grid()
plt.plot(xg, yg)
plt.xlabel('x')
plt.ylabel('y')
plt.title('f(x)')
plt.show()
a, b=eval(input("Введите границы отрезка через пробел (a<b): "))
ε=float(input("Введите точность вычисления: "))
n=numbers_after_point(ε)
φ=(x+5)**(1/3)
print(f'φ={φ}')
xg = np.linspace(a, b, 20)
yg = [diff(φ).subs(x, i) for i in xg]
plt.grid()
plt.plot(xg, yg)
plt.xlabel('x')
plt.ylabel('y')
plt.title("Производная от φ(x)")
plt.show()
xg = np.linspace(a, b, 20)
yg = [φ.subs(x, i) for i in xg]
plt.grid()
plt.plot(xg, yg)
plt.xlabel('x')
plt.ylabel('y')
plt.title("φ(x)")
plt.show()
if abs(diff(φ, x).subs(x, a))<1 and abs(diff(φ, x).subs(x, b))<1 and φ.subs(x, a)>=a and φ.subs(x, a)<=b and φ.subs(x, b)>=a and φ.subs(x, b)<=b and y.subs(x, a)*y.subs(x, b)<0:
	x1=a
	print(f"x0={x1}")
	k=0
	while True:
		x2=φ.subs(x, x1)
		k+=1
		print(f'x{k}={round(x2, n+1)}, |x{k}-x{k-1}| = {round(abs(x2-x1), n+1)}')
		if (abs(x2-x1)<ε) and (isclose(abs(x2-x1), ε)==False):
			print(f'x = {round(x2, n+1)}')
			break
		else:
			x1=x2
else:
	print('Функция φ не удовлетворяет условиям сходимости метода простой итерации или корня уравнения на данном отрезке нет')	
```
## **The English language**
Level of the English language is not high.
