# Python-Libraries

<h1>📦 NumPy (Numerical Python)</h1>
<p><b>NumPy</b> is a Python library used for numerical computing and multi-dimensional arrays.</p>

<pre><code>import numpy as np</code></pre>

<hr>

<h2>🧱 NumPy Array</h2>

<h3>🔹 array()</h3>
<p>Creates a NumPy array from a list or tuple.</p>

<pre><code>a = np.array([1, 2, 3, 4])
print(a)</code></pre>

<div class="output">
[1 2 3 4]
</div>

<hr>

<h2>🔢 Array Creation Functions</h2>

<h3>🔹 arange()</h3>

<pre><code>a = np.arange(1, 10, 2)
print(a)</code></pre>

<div class="output">
[1 3 5 7 9]
</div>

<h3>🔹 zeros()</h3>

<pre><code>z = np.zeros((2, 3))
print(z)</code></pre>

<div class="output">
[[0. 0. 0.]
 [0. 0. 0.]]
</div>

<h3>🔹 ones()</h3>

<pre><code>o = np.ones((3, 2))
print(o)</code></pre>

<div class="output">
[[1. 1.]
 [1. 1.]
 [1. 1.]]
</div>

<h3>🔹 fill() / full()</h3>

<pre><code>f = np.full((2, 2), 7)
print(f)</code></pre>

<div class="output">
[[7 7]
 [7 7]]
</div>

<h3>🔹 eye()</h3>

<pre><code>i = np.eye(3)
print(i)</code></pre>

<div class="output">
[[1. 0. 0.]
 [0. 1. 0.]
 [0. 0. 1.]]
</div>

<hr>

<h2>📐 Array Properties</h2>

<h3>🔹 ndim</h3>

<pre><code>a = np.array([[1,2,3],[4,5,6]])
print(a.ndim)</code></pre>

<div class="output">2</div>

<h3>🔹 shape</h3>

<pre><code>print(a.shape)</code></pre>

<div class="output">(2, 3)</div>

<h3>🔹 size</h3>

<pre><code>print(a.size)</code></pre>

<div class="output">6</div>

<hr>

<h2>🔄 Reshape</h2>

<h3>🔹 reshape()</h3>

<pre><code>a = np.arange(6)
print(a.reshape(2,3))</code></pre>

<div class="output">
[[0 1 2]
 [3 4 5]]
</div>

<h3>🔹 reshape(-1,1)</h3>

<pre><code>a = np.array([1,2,3,4])
print(a.reshape(-1,1))</code></pre>

<div class="output">
[[1]
 [2]
 [3]
 [4]]
</div>

<h3>🔹 reshape(1,-1)</h3>

<pre><code>print(a.reshape(1,-1))</code></pre>

<div class="output">
[[1 2 3 4]]
</div>

<hr>

<h2>🔃 Array Operations</h2>

<h3>🔹 ravel()</h3>

<pre><code>a = np.array([[1,2],[3,4]])
print(a.ravel())</code></pre>

<div class="output">
[1 2 3 4]
</div>

<h3>🔹 transpose()</h3>

<pre><code>print(a.transpose())</code></pre>

<div class="output">
[[1 3]
 [2 4]]
</div>

<h3>🔹 diagonal()</h3>

<pre><code>a = np.array([[1,2,3],[4,5,6],[7,8,9]])
print(a.diagonal())</code></pre>

<div class="output">
[1 5 9]
</div>

<h3>🔹 concatenate()</h3>

<pre><code>a = np.array([1,2])
b = np.array([3,4])
print(np.concatenate((a,b)))</code></pre>

<div class="output">
[1 2 3 4]
</div>

<hr>

<h2>🎲 Random Functions</h2>

<h3>🔹 randint()</h3>

<pre><code>print(np.random.randint(1, 10, 5))</code></pre>

<div class="output">
[3 7 1 9 5]
</div>

<h3>🔹 randn()</h3>

<pre><code>print(np.random.randn(3))</code></pre>

<div class="output">
[-0.45  1.32  0.78]
</div>

<h3>🔹 random()</h3>

<pre><code>print(np.random.random(4))</code></pre>

<div class="output">
[0.23 0.89 0.45 0.67]
</div>

<hr>

<h2>📊 Statistical Functions</h2>

<pre><code>a = np.array([10, 20, 5])</code></pre>

<div class="output">
max → 20  
min → 5  
sum → 35  
argmax → 1  
argmin → 2
</div>

<hr>

<h2>✖️ Matrix Multiplication</h2>

<pre><code>a = np.array([[1,2],[3,4]])
b = np.array([[5,6],[7,8]])

print(np.matmul(a,b))</code></pre>

<div class="output">
[[19 22]
 [43 50]]
</div>
<pre><code>a = np.array([10, 20, 5])</code></pre>

<h3>🔹 max()</h3>
<pre><code>print(a.max())</code></pre>
<div class="output">20</div>

<h3>🔹 min()</h3>
<pre><code>print(a.min())</code></pre>
<div class="output">5</div>

<h3>🔹 sum()</h3>
<pre><code>print(a.sum())</code></pre>
<div class="output">35</div>

<h3>🔹 argmax()</h3>
<pre><code>print(a.argmax())</code></pre>
<div class="output">1</div>

<h3>🔹 argmin()</h3>
<pre><code>print(a.argmin())</code></pre>
<div class="output">2</div>

<hr>

<h2>🔁 repeat()</h2>

<pre><code>a = np.array([1, 2, 3])
print(np.repeat(a, 2))</code></pre>

<div class="output">
[1 1 2 2 3 3]
</div>

<hr>

<h2>🧭 Axis Operations</h2>

<pre><code>a = np.array([[1, 2],
              [3, 4]])</code></pre>

<h3>🔹 axis = 0 (Column-wise)</h3>

<pre><code>print(a.sum(axis=0))</code></pre>

<div class="output">
[4 6]
</div>

<h3>🔹 axis = 1 (Row-wise)</h3>

<pre><code>print(a.sum(axis=1))</code></pre>

<div class="output">
[3 7]
</div>

<hr>

<h2>➕ Arithmetic Operations</h2>

<h3>🔹 add()</h3>

<pre><code>a = np.array([1, 2])
b = np.array([3, 4])

print(np.add(a, b))</code></pre>

<div class="output">
[4 6]
</div>

<hr>

<h2>🧮 Math Functions</h2>

<pre><code>a = np.array([1, 4, 9])</code></pre>

<h3>🔹 sqrt()</h3>
<pre><code>print(np.sqrt(a))</code></pre>
<div class="output">
[1. 2. 3.]
</div>

<h3>🔹 log()</h3>
<pre><code>print(np.log(a))</code></pre>
<div class="output">
[0.         1.38629436 2.19722458]
</div>

<h3>🔹 exp()</h3>
<pre><code>print(np.exp(a))</code></pre>
<div class="output">
[2.71828183 54.59815003 8103.08392758]
</div>




