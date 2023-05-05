Download Link: https://assignmentchef.com/product/solved-ct5132-ct5148-lab-week-03
<br>






Solutions are available in the /code directory in our .zip.

<ol>

 <li>Last week we calculated a list containing <em>e<sup>x </sup>∀x ∈ </em>[0<em>.</em>0<em>,</em>0<em>.</em>1<em>,…,</em>1<em>.</em>0], using range, lambda, map and math.exp. Now, let’s do the Numpy way, using np.linspace and np.exp. Solution: exp_np.py.</li>

 <li>In the ECG (heartbeat) example, we saw how to use a Boolean expression to give a new array telling us where the Boolean expression is true:</li>

</ol>

<table width="632">

 <tbody>

  <tr>

   <td width="632">x <strong>= </strong>np.array([<strong>–</strong>3, -2, -1, 0, 1, 2, 3]) x <strong>&gt; </strong>0<em># array([False, False, False, False, True, True, True])</em></td>

  </tr>

 </tbody>

</table>

We can also create a new array consisting of the values where it is true:

x <strong>= </strong>np.array([<strong>–</strong>3, -2, -1, 0, 1, 2, 3]) x[x <strong>&gt; </strong>0]

<em># array([1, 2, 3])</em>

We can use the same idea now on the left-hand side of an assignment, to overwrite only values in an array where the Boolean expression is true. Use this to set all negative values in x to zero. Solution: numpy_boolean_lhs.py.

<ol start="3">

 <li>Find the biggest jump between any two consecutive values in the heartbeat (ECG) data. When does it occur? What were the before and after values? Hint: recall we have seen np.diff and np.argmax. I suggest np.diff(x, prepend=x[0]) this time instead of prepend=0. Solution: heartbeat_jump.py.</li>

 <li>Use Numpy to create a “chessboard” pattern like this:</li>

</ol>

[[0 1 0 1 0 1 0 1]

[1 0 1 0 1 0 1 0]

<ul>

 <li>1 0 1 0 1 0 1]</li>

 <li>0 1 0 1 0 1 0]</li>

 <li>1 0 1 0 1 0 1]</li>

 <li>0 1 0 1 0 1 0]</li>

 <li>1 0 1 0 1 0 1]</li>

 <li>0 1 0 1 0 1 0]]</li>

</ul>

Hints: use np.linspace, np.meshgrid, and the % operator. For the final touch, look up astype so that your array is int-valued, not float. Solution: chessboard.py.

1

<ol start="5">

 <li>Create the 2d array <em>a<sub>ij</sub></em>, a “vertical” 1d array <em>b<sub>i</sub></em>, a “horizontal” 1d array <em>c<sub>j</sub></em>, and a scalar <em>d</em>. Calculate the new 2d array <em>q </em>where <em>q<sub>ij </sub></em>= <em>a<sub>ij </sub></em>+<em>b<sub>i </sub></em>+<em>c<sub>j </sub></em>+<em>d</em>. (This scenario will be familiar to CT5141 Optimisation students as it occurs in linear objective functions.) Solution: 2d_1d_scalar.py.</li>

</ol>

<table width="632">

 <tbody>

  <tr>

   <td width="53">a: 9 5</td>

   <td width="35">1</td>

   <td width="63">b: 10</td>

   <td width="126">c: 100 200 300</td>

   <td width="70">d: 1000</td>

   <td width="286">q: 1119 1215 1311</td>

  </tr>

  <tr>

   <td width="53">4 3</td>

   <td width="35">8</td>

   <td width="63">20</td>

   <td width="126"></td>

   <td width="70"></td>

   <td width="286">1124 1223 1328</td>

  </tr>

  <tr>

   <td width="53">2 7</td>

   <td width="35">6</td>

   <td width="63">30</td>

   <td width="126"></td>

   <td width="70"></td>

   <td width="286">1132 1237 1336</td>

  </tr>

 </tbody>

</table>

<ol start="6">

 <li>In our fractals example, we claimed that when a point “escapes” from a circle of radius 2, it will never come back, but in test_escape_and_return(), that’s exactly what seemed to happen. Why? Solution: fractal_escape_and_return.py.</li>

 <li>Try different values for zmin and zmax in the Julia example. What is the effect?</li>

 <li>Try different values for c. Do you get any interesting images? I liked c = -0.015 + 0.66j.</li>

 <li>Try different colourmaps in the Julia set. Look up:</li>

</ol>

https://matplotlib.org/3.1.0/tutorials/colors/colormaps.html

to see a gallery.

2