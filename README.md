# Just_for_fun
### 学习《大话数据结构》
#### Day1 <br>
##### 数据结构:
- 是相互之间存在一种或多种特定关系的数据元素的集合
- 研究非数值计算的程序设计问题中的操作对象,以及他们之间的关系和操作等相关问题的学科 <br>
##### 数据:
- 是描述客观事物的符号,是计算机中可以操作的对象,是能被计算机识别,并输入给计算机处理的符号的集合
- 数据项是数据不可分割的最小单元 <br>
##### 数据结构分为逻辑结构与物理结构:
- 逻辑结构: 集合结构, 线性结构, 树形结构, 图形结构
- 物理结构: 数据的逻辑结构在计算机中的处理形式 链式存储结构, 顺序存储结构 <br>
##### 链式存储结构:
- 是把数据元素存放在任意的存储单元里,这组存储单元是连续的,也可以是不连续的 <br>

#### Day2
##### 算法设计:
- 正确性
- 可读性
- 健壮性
- 时间效率高和存储量低
##### 算法的五个基本特性
- 输入
- 输出
- 有穷性
- 确定性
- 可行性

##### 算法效率的度量方法(把程序看成是独立于程序设计语言的算法或系列步骤)
- 事后统计法
- 事前分析估算法

##### 算法效率的判断
- 函数中的常数和其他次要项常常可以忽略,而更应该关注主项(最高阶项)的阶数
##### 大O记法 O()
- O(1)< O(logn) < O(n) < O(nlogn) < O(n²) < O(n³) < O(2ⁿ) < O(n!) < O(nⁿ)
<table>
  <tr><td>O(1)</td><td>常数阶</td></tr>
  <tr><td>O(n)</td><td>线性阶</td></tr>
  <tr><td>O(n²)</td><td>平方阶</td></tr>
  <tr><td>O(logn)</td><td>对数阶</td></tr>
  <tr><td>O(2ⁿ)</td><td>指数阶</td></tr>
  <tr><td>O(nlogn)</td><td>nlogn阶</td></tr>
  <tr><td>O(n³)</td><td>立方阶</td></tr>
</table>


#### Day3
##### 线性表
- 线性表是零个或多个数据元素的优先序列
- 线性表元素的个数n(n≥0)定义为线性表的长度,当n=0时, 称为空表 
- 在较复杂的线性表中, 一个数据元素可以由若干个数据项组成
##### 线性表的顺序存储结构
- 线性表的顺序存储结构, 值得是用一段地址连续的存储单元依次存储线性表的数据元素
- 顺序存储结构需要三个属性:
  - 存储空间的起始位置 - 线性表的最大存储容量 - 线性表的当前长度
  - 每个线性表位置的存入或者取出数据,对于计算机来说都是相等的时间,也就是一个常数,存取时间性能为O(1), 
  通常我们把具有这一特点的存储结构称为*随机存储结构*
- 插入算法的思路:
  - 如果插入位置不合理, 抛出异常
  - 如果线性表长度大于数据长度, 则抛出异常或动态增加容量
  - 从最后一个元素开始向前遍历到第i个位置, 分别将它们都向后移动一个位置
  - 将要插入元素填入位置i处
  - 表长加1
- 删除算法的思路:
  - 删除位置不合理, 抛出异常;
  - 取出删除元素;
  - 从删除元素位置开始遍历到最后一个元素, 分别将它们都向前移动一个位置
  - 表长减1
##### 线性表结构的优缺点
<table>
  <tr><td>优点</td><td>缺点</td></tr>
  <tr><td>无须为表示表中元素之前的逻辑关系而增加额外的存储空间</td><td>插入和删除操作需要移动大量的元素</td></tr>
  <tr><td>可以快速地存取表中任一位置的元素</td><td>当线性表长度变化较大时,难以确定存储空间的容量</td></tr>
  <tr><td></td><td>造成存储空间的"碎片"</td></tr>
</table>

##### 单链表
- n个结点(ai的存储映像)链结成一个链表, 即为线性表(a1, a2, ..., an)的链式存储结构, 因为链表的每个结点中只包含一个指针域, 所以叫做单链表
- 存取复杂度O(n)
- 插入删除O(n)如果插入多个,后面O(1)

 
