# 第一周作业总结
#### 练习过的题目
1. LC_01_TwoSum 
    + 在思考思路的时候，因为之前老师讲解过，可以使用双指针的方式去将双循环将为单循环，
        但是最后考虑到，如果需要排序的话，那么返回的数组下标将不准确, 所以如果用这种双指针法去降低时间复杂度，
        还需要使用数组或者哈希辅助记录原来元素的数组，在确定目标数据之后，再取出元素的旧下标，返回；
        这样就是牺牲空间复杂度，来换取时间(也有可能会带来源码层面更大的时间复杂度消耗),故此路不通
    + 另外，在leetcode的国内站点或者国际站都出现用辅助哈希来降低时间复杂度为O(n), 但是这种解法的时间复杂度
        并不为O(n), 在计算时间复杂度的时候，直接忽略了jdk源码处理哈希所带来的消耗
2. LC_11_ContainWithMostWater
    + 解法除了暴力枚举，还用到了双指针法，从边界遍历夹逼，寻找目标元素输出；并且双边指针也是根据计算结果来动态移动，
        这种方式比较巧妙
3. LC_15_ThreeSum
    + 3sum的暴力枚举写出来的代码超出来leetcode的时间限制
    + 双指针法将O(n^3)的复杂度将为O(n^2); 我觉得其中巧妙的地方处理使用双指针的方式去寻找元素之外，
        还有就是在双边指针移动的时候，很巧妙的利用了java运算的方式去避免相同值的元素重复计算`while (i < j && nums[i] == nums[++i]);`
4. LC_26_RemoveDuplicatesFromSortedArray
    + 使用指针标记确认了非重复元素的位置，并在符合条件的时候，往后移动这个指针，数据只变更标记后面的元素信息；
        题目要求直接返回非重复元素的个数，所以直接将这个指针+1返回即可
5. LC_70_ClimbingStairs
    + 爬楼梯是一个涉及到动态规划的问题，这个题目对动态规划对感受不是很深，
        所以对斐波那契数列的规则计算的方式比较容易理解；而动态规划的算法，后面需要更加深刻的理解并练习
6. LC_283_MoveZeroes
    + 移动0位置这道题，当初自己写的时候，使用了swap来对调两个元素的位置，但是其实看了discuss之后，发现主要关注非0元素位置即可，而0元素位不需要处理

#### 个人总结
+ 在预习周学习了刷题技巧之后，本周跟着老师的课程，实战进入了leetcode的刷题状态，避免了像以前一样，
    一道题看了题目之后，就埋头思考解法，结果耗费了很多时间，产生了自己一定要解出来，不然就是能力的问题，
    就这样陷入了死胡同，一直以来的挫败感压抑着，心中产生了对刷题特别是算法题的畏惧；而这两周的刷题技巧实战，
    让我纠正了这种心理
+ 另外针对解题技巧，也积累了万能的暴力循环法、双指针法、还有遇到没头绪的题目可以用列举进行归纳找规律等思路，很受用
+ 不过，反思了一下这周的算法学习以及刷题时间，这周自己都是在晚上十点以后，或者周末这种能够有大片时间的时段来学习及刷题
    这样的话，既然自己无法利用碎片时间让自己学习，那就合理安排这种一大段时间来系统学习算法，只有这样静下来连续学习，
    才能系统的建立自己的知识架构；希望这个可能让我养成这个习惯，以后运用到别的专业知识的学习上

  

