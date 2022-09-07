# a-simple-constructive-proof-of-Simultaneous-diagonalization-theorem
a simple constructive proof of Simultaneous diagonalization theorem in quantum computing.

(Simultaneous diagonalization theorem) Suppose $A$ and $B$ are Hermitian operators. Then $[A, B] = 0$ if and only if there exists an orthonormal basis such that both $A$ and $B$ are diagonal with respect to that basis. We say that $A$ and $B$ are simultaneously diagonalizable in this case.

Proof : 

We  can construct a new operator $M=A+iB$,

Then,we prove that if $A$ and $B$ are Hermitian operators,  $AB=BA$ $\Leftrightarrow$ $M$ is normal, which says that $MM^\dagger=M^\dagger M$ $\Leftrightarrow$ $A$ and $B$ are simultaneously diagonalizable。

Firstly，we prove that  $AB=BA \Leftrightarrow MM^\dagger=M^\dagger M$:

​	 $MM^\dagger=(A+iB)(A-iB)=A^2+B^2+i(BA-AB)$

​	$M^\dagger M=(A-iB)(A+iB)=A^2+B^2+i(AB-BA)$	

​	if $AB=BA$, we can get $MM^\dagger=M^\dagger M$

​	if  $MM^\dagger=M^\dagger M$, we can  get $AB=BA$.

Secondly, we prove that $MM^\dagger=M^\dagger M$ $\Leftrightarrow$  $A$ and $B$ are simultaneously diagonalizable:

​	if $MM^\dagger=M^\dagger M$ , according to spectral decomposition theorem, we can write $M$ as

$M = \sum_j \lambda_j |j\rangle \langle j|$,where $\lambda_i$ are the eigenvalues of $M$, $|j\rangle$ is an orthonormal basis. Then we can write $M^\dagger=\sum_j \lambda_j^* |j\rangle \langle j|$, so we get $A= (M+M^\dagger)/2=\sum_j \frac{(\lambda_j+\lambda^*_j)}{2} |j\rangle \langle j|$,

$B=(M-M^\dagger)/(2i)=\sum_j \frac{(\lambda_j-\lambda^*_j)}{2i} |j\rangle \langle j|$, $A$ and $B$ are simultaneously.

​	if $A$ and $B$ are simultaneously diagonalizable, we can write $A =\sum_j \alpha_j|j\rangle \langle j|,B=\sum_j \beta_j |j\rangle \langle j|$, so $M=A+iB=\sum_j (\alpha_j+i\beta_j) |j\rangle \langle j|$ ,

according to spectral decomposition theorem, $M$ is normal, which is that $MM^\dagger=M^\dagger M$。                              																								 $\square$

Yu Chen
chenyu21b@ict.ac.cn
ICT,CAS
