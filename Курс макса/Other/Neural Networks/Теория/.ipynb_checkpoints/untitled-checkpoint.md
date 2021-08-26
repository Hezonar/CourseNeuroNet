1. Постройте граф вычислений и найдите производную $\frac{\partial f}{\partial x}$ для функции $$f(h(x))$$

    *Ответ*:
    $$\frac{\partial f}{\partial h}*
\frac{\partial h}{\partial x}$$
    
    ![ответ](backprop_answers/1.png)


2. Постройте граф вычислений и найдите производную $\frac{\partial f}{\partial x}$ для функции $$f(h(x), g(x))$$

    *Ответ*:
    
    $$\frac{\partial f}{\partial h}*
\frac{\partial h}{\partial x} 
+ 
\frac{\partial f}{\partial g}*
\frac{\partial g}{\partial x}$$

    ![ответ](backprop_answers/2.png)


3. Постройте граф вычислений и найдите производную по $x$ для функции $$f(h(w(x), y(x)), g(y(x), z(x)))$$

    <details>
      <summary markdown="span">Ответ</summary>

      $$\frac{\partial f}{\partial h}*(
      \frac{\partial h}{\partial w}*\frac{\partial w}{\partial x}+
      \frac{\partial h}{\partial y}*\frac{\partial y}{\partial x})
      + 
      \frac{\partial f}{\partial g}*(
      \frac{\partial g}{\partial y}*\frac{\partial y}{\partial x}
      +
      \frac{\partial g}{\partial z}**\frac{\partial z}{\partial x})$$

      ![ответ](backprop_answers/3.png)
    </details>
    
4. Даны функции: 
    $$a=w_{ab}*b+w_{ac}*c+w_{ad}*d+w_{a},$$
    $$b=w_{bx}*x+w_{b},$$
    $$c=w_{cx}*x+w_{c},$$
    $$d=w_{dx}*x+w_{d};$$
    
    1) Найдите производные $\frac{\partial a}{\partial b}$, $\frac{\partial a}{\partial c}$, $\frac{\partial a}{\partial d}$, $\frac{\partial b}{\partial x}$, $\frac{\partial c}{\partial x}$, $\frac{\partial d}{\partial x}$;
    
    2) Постройте граф вычислений и найдите производную $\frac{\partial a}{\partial x}$ (без подстановки из шага 1);
    
    3) Используя предыдущии шаги, найдите производную $\frac{\partial a}{\partial x}$.
    
    4) Используя предыдущии шаги, найдите производные $\frac{\partial a}{\partial w_{ab}}$, $\frac{\partial a}{\partial w_{ac}}$, $\frac{\partial a}{\partial w_{ad}}$, $\frac{\partial a}{\partial w_{a}}$, $\frac{\partial a}{\partial w_{bx}}$, $\frac{\partial a}{\partial w_{b}}$, $\frac{\partial a}{\partial w_{cx}}$, $\frac{\partial a}{\partial w_{c}}$, $\frac{\partial a}{\partial w_{dx}}$, $\frac{\partial a}{\partial w_{d}}$.