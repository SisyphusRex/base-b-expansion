# base-b-expansion
Implementation of base b expansion algorithm.

## What is
For an integer b > 1.  Every positive integer n can be expressed uniquely as:  
$`𝑛 = 𝑎_{𝑘} * 𝑏^{𝑘} + 𝑎_{𝑘-1} * 𝑏^{𝑘-1}+...𝑎_{1} * 𝑏^{1} + 𝑎_{0} * 𝑏^{0}`$  
Where $`𝑎_{𝑘}`$ is the digit and $`𝑏^{𝑘}`$ is the power of the base.  
256 base 10:  
$`2*10^{2} + 5*10^{1} + 6*10^{0}`$  

Base b expansion of n:  
$`(𝑎_{𝑘}𝑎_{𝑘-1}...𝑎_{1}𝑎_{0})_{𝑏}`$

## Pseudocode
Input: Integers n and b. b > 1 and n ≥ 1  
Output: base b expansion of n.  base b digits are output in reverse order  

* x = n
* while (x > 0)
  * output(x mod b)
  * x = x div b
