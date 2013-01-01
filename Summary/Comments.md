Comments
=====================================



Determining the transition redshift means determining the Hubble function in most methods. So why not write down the whole deceleration history and find which point is better to use. By 'better' I mean deviating the most from some standard model, which can be described by functional derivative. (I am not completely sure about this. Functional analysis means the derivative along the function in mathematics.)


So my idea is to check the functional derivative.

First of all, we have to calculate the functional derivative of an example.

Assume 

\[ F[w(z)] = e^{ 3\int_0^z \frac{1+w(\tilde z)}{1+\tilde z} } \mathrm d\tilde z \]

The functional derivative of \(F[w(z)]\)

 \begin{eqnarray}
\frac{\delta F[w(\tilde z)]}{\delta w(y)} &=& \lim _ {\epsilon \rightarrow 0} \frac{ F[w(\tilde z) +\epsilon \delta(\tilde z - y) ] - F[w(\tilde z)]  }{ \epsilon } \newline
&=& \lim _ {\epsilon \rightarrow 0}  \frac{ \exp(3\int _ 0 ^ z \frac{1 + w (\tilde z) + \epsilon \delta(\tilde z - y)}{1+\tilde z}\mathrm d\tilde z ) - \exp( 3\int _ 0 ^ z \frac{1 + w(\tilde z)}{1+\tilde z} \mathrm d\tilde z ) }{ \epsilon } \newline
&=& \lim _ {\epsilon \rightarrow 0} \frac{ \exp(3\int _ 0 ^ z \left ( \frac{1 + w(\tilde z)}{ 1 + \tilde z } + \frac{ \epsilon \delta ( \tilde z - y ) }{ 1 + \tilde z }\right) \mathrm d \tilde z ) - \exp(3\int _ 0 ^ z \frac{1 + w(\tilde z)}{1+\tilde z} \mathrm d\tilde z   ) }{\epsilon} \newline
&=& \lim _ {\epsilon \rightarrow 0 } \frac{ \exp(3\int _ 0 ^ z \frac{1+w(\tilde z)}{1+\tilde z}\mathrm d \tilde z) \exp(3\int _ 0 ^ z \frac{\epsilon \delta(\tilde z - y)}{1+tilde z}\mathrm d\tilde z) - \exp(3\int _ 0 ^ z \frac{1 + w(\tilde z)}{1+\tilde z} \mathrm d\tilde z   ) }{ \epsilon } \newline
&=&\exp\left(3\int _ 0 ^ z \frac{1+w(\tilde z) }{ 1+ \tilde z }\mathrm d\tilde z\right)\lim _ {\epsilon \rightarrow 0} \frac{ \exp\left( 3\int _  0 ^ z \frac{\epsilon \delta(\tilde z - y)}{1+\tilde z}\mathrm d \tilde z  \right) -1 }{\epsilon} \newline
&=& F[w(\tilde z)] \lim _ {\epsilon \rightarrow 0} \frac{\exp\left( \frac{3\epsilon}{1+y} \right) - 1}{\epsilon} \newline
&=& F[w(\tilde z)] \frac{3}{1+y} \newline
&=&F[w(\tilde z)] \frac{3}{1+z}
\end{eqnarray}


Deceleration parameter $q$ is defined as

\[ q[w(z)] \equiv -1 - \frac{\dot H[w(z)]} {H[w(z)]^2} \]

Let's check the functional derivative of \(H[w(z)]\) first. Here we use delta function as test function to calculate the derivative.



















