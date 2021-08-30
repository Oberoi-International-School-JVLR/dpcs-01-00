# Unit 01: First programs
## Lab 00: Practice with Computational Algorithms


---

**Directions**
In this lab, you will need to complete the following tasks. Make sure that you complete each in their respective files. Questions should be answered in the `Questions.md` file.

---

### Heron's Method

Modify the `heron.html` file to include:

1. A label for the output of your calculation to make it clear what the value represents. (Visual Feedback to the user.)

2. An additional user input and related JavaScript for allowing the user to set a tolerance for the output. Include a default value (0.001).

---

### Euclid's Algorithm

Modify the `euclid.html` to implement the following algorithm for finding Greatest Common Divisors. 

**Algorithm**

Given two positive integers, `a` and `b` such that `a >= b`:

1. If `a = b`, output `a`
2. Otherwise, set `a = b` and `b = a - b`
3. Repeat from Step #1 until `a = b`.

(You might want to verify this works with a simple example, done by hand, such as `a = 20` and `b = 12` )

**Note:** Because the single `=` is already used to *assign* values in JavaScript, a *test for equality* requires two: `==`.

Example: `(a = b)` will set the value of `a` to the value of `b`, but `(a == b)` will test if the values are equal.

---

### Numerical Differentiation
In mathematics, the *derivative* of a function is the slope, or rate of change, of a function at a particular point. While Calculus provides details on how to calculate this value precisely, the computer can be used to derive a very good estimate.

Consider: the *derivative of a function, `f`, at a particular point, `n`, called `df(n)`* can be estimated as the slope of a line connecting points on `f` very close to `n`. That is, for some small distance, `h`, from `n`, we can calculate the slope as:

$$d_f(n) = \frac{f(n + h) - f(n)}{h}$$

The process of finding these values is known as *differentiation*.

**Extra:** Convince yourself this formula is equivalent to the slope formula: 

$$m = \frac{\Delta y}{\Delta x}$$

Modify `ndiff.html` to calculate the numerical derivative at a user-supplied point for the function:

$$f(x) = 3x^2 + \frac{2}{x} + 7$$

To assist your tests, here are the **exact** values for the derivative of this function at particular points. (**Note:** Remember, your values should be good *estimates* of these values.)

| `n` | `df(n)` |
|:---:|:---:|
|2 | 11.5 |
|5 | 29.92 |
| -3 | -18.222... |

**Note:** The function you create here will gain significant power in a few lessons, once we discuss clever ways to represent general algebraic functions in JavaScript. Be prepared to revisit this exercise after that!
