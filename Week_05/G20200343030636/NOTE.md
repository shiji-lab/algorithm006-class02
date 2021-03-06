动态规划
1.核心是状态的定义，一个正确的DP状态应该符合以下几点
A.状态或者通过对状态的简单运算能直接对应到问题的答案，运算通常是max，min，sum等方式，过程中不需要再去求解其他问题；
B.状态的定义和问题的规模无关，不会随着规模的变化影响到状态的定义，通常求解大规模的问题可以分成先求解小规模的问题，所以动态规划中，分治是一种重要的思路；
C.每一个具体规模的状态值，都不受其他因素的影响；
D.状态表通常是归纳总结状态方程的重要方式；
E.当一个状态无法解决问题时，尝试定义多个状态；
F.DP中，经常会需要额外的空间来存储小规模的解，但有一些可以通过优化状态方程或者压缩来进行空间优化；例如斐波拉切数列，一般解法但空间复杂度是O(n)，但经过空间压缩优化，
可以到O(1)的空间复杂度
G.有一些问题，可以用一套状态方程来解决，例如打家劫舍问题，股票问题，戳气球问题等；
H.求最值（最大，最小，最短），能否达成，总数（路径总数)常常可以考虑用DP来解决，但有一些用贪心来解决会更快更优；