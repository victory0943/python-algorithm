## 1. 字母大小写全排列  -- 784-letter_case_permutation

- 来源： leetcode 784 -- easy
- 问题： 给定一个字符串S，通过将字符串S中的每个字母转变大小写，我们可以获得一个新的字符串。返回所有可能得到的字符串集合。

### 思路1：

在回溯过程中，每次都添加有变化的字符串到数组arr中， 最后返回arr

## 2. 二进制手表 -- easy

- 来源：**leetcode 401**
- 问题： 二进制手表顶部有 4 个 LED 代表小时（0-11），底部的 6 个 LED 代表分钟（0-59）。每个 LED 代表一个 0 或 1，最低位在右侧。 给定一个非负整数 n 代表当前 LED 亮着的数量，返回所有可能的时间。


## 3.  子集 -- sub_set

- 来源： [leetcode 78](https://leetcode-cn.com/problems/subsets/)

- 题目： 给定一组不含重复元素的整数数组 nums，返回该数组所有可能的子集。
- 说明：结果不能包含重复的子集。

- 举例： nums = [1,2,3]; 结果为：[[], [1], [1,2], [1,2,3], [1,3], [2], [2,3], [3]]

### 思路1：回溯法

采用回溯法生成子集，即对于每个元素，都有试探放入或不放入集合的两个选择.
**注意： python 与 c++ 的实现方式有所不同，原因在于，python 的result 中存储的是对象的地址，如果对象发生改变，那么result就发生了变化**


## 4. 括号生成

- 来源：[leetcode 22](https://leetcode-cn.com/problems/generate-parentheses/)
- 题目： 给出 n 代表生成括号的对数，请你写出一个函数，使其能够生成所有可能的并且有效的括号组合。
- 举例：输入n=3， 则输出: 
```
[
  "((()))",
  "(()())",
  "(())()",
  "()(())",
  "()()()"
]
```

- 思路： 
> - 什么时候返回：n == 0
> - 什么时候将该可能加入到结果数组result中： n==0 and left_num == right_num
> - 什么情况符合，什么情况不符合: left_num 的数目不能大于 right_num 的数目

## 5. 全排列

- 来源： leetcode 46
- 题目： 给定一个没有重复数字的序列，返回其所有可能的全排列。

- 思路：


## 6. 组合
- 来源： **leetcode 77**
- 问题： 给定两个整数 n 和 k，返回 1 ... n 中所有可能的 k 个数的组合。
- 思路：
- 注意： 需要进行优化才能通过


## 7. 组合总和3
- 来源： leetcode 216
- 题目：找出所有相加之和为 n 的 k 个数的组合。组合中只允许含有 1 - 9 的正整数，并且每种组合中不存在重复的数字。
- 说明： 所有数字都是正整数， 解集中不能包含重复的组合


## 8. 组合总和

- 来源：leetcode 40

- 题目： 给定一个数组 candidates 和一个目标数 target ，找出 candidates 中所有可以使数字和为 target 的组合。

- 说明：
  > - candidates 中的每个数字在每个组合中只能使用一次。
  > - 所有数字（包括目标数）都是正整数。
  > - 解集不能包含重复的组合。 

## 9. 分割回文串

- 来源： **leetcode 131**
- 问题：给定一个字符串s， 将s分割成一些子串，使得每个字串都是回文串

## 10. 组合总和 2

- 来源： leetcode 40
- 问题： 给定一个数组 candidates 和一个目标数 target ，找出 candidates 中所有可以使数字和为 target 的组合。candidates 中的每个数字在每个组合中只能使用一次。
- 说明： 所有数字都是正整数， 解集中不能包含重复的组合

## 11. 子集

- 来源： leetcode 90
- 题目：给定一个可能包含重复元素的整数数组 nums，返回该数组所有可能的子集（幂集）。
- 说明：解集不能包含重复的子集。
- 举例： 输入： [1,2,2]， 输出： 
  [  [2], [1], [1,2,2], [2,2], [1,2], [] ]
- **注意：** [2,1,2] 与 [1,2,2] 是重复的子集

## 12. 全排列2

- 来源： leetcode 47
- 题目： 给定一个可包含重复数字的序列，返回所有不重复的全排列。




## 5. N皇后问题

- **来源：[leetcode 51](https://leetcode-cn.com/problems/n-queens/)**
- 问题：n 皇后问题研究的是如何将 n 个皇后放置在 n×n 的棋盘上，并且使皇后彼此之间不能相互攻击。 下图为8皇后的一种解法
![](http://ww1.sinaimg.cn/large/006gOeiSly1g0vhda5ra5j307607o748.jpg)
    给定一个整数 n，返回所有不同的 n 皇后问题的解决方案。每一种解法包含一个明确的 n 皇后问题的棋子放置方案，该方案中 'Q' 和 '.' 分别代表了皇后和空位。

- 举例： 输入：4， 输出：
```
[
 [".Q..",  // 解法 1
  "...Q",
  "Q...",
  "..Q."],

 ["..Q.",  // 解法 2
  "Q...",
  "...Q",
  ".Q.."]
]
```
