---
title: ListNode
comments: true
date: 2020-12-02 02:36:27
updated: 2020-12-02 02:36:27
categories: Data Structure
tags: [List, Note]
---

*凡是遇上带指针结构的基本上都能用迭代和递归解决*

##### 迭代
>时间复杂度: O(n)
>空间复杂度: O(1)
>思路清晰但代码容易复杂

##### 递归
>时间复杂度: O(n)
>空间复杂度: O(n) ***堆栈结构***
>相信定义，画图会好理解很多。一定要注意 *base case*(可以先留白)和 *return value*
<!--More-->

***

##### ReverseList

```java
class Solution {
    public ListNode reverseList(ListNode head) {
        // 记录下一节点， 当前节点指向上一节点
        // 同时下移上一节点和当前节点，当curr为
        // null时，返回逆转后的头部即prev
        ListNode prev = null;
        ListNode curr = head;
        while(curr != null) {
            ListNode temp = curr.next;
            curr.next = prev;
            prev = curr;
            curr = temp;
        }
        return prev;
    }
}
```
```java
class Solution {
    public ListNode reverseList(ListNode head) {
        // 递归一定要有base case
        // 当只有一个节点或者没有时返回本身
        if (head == null || head.next == null) {
            return head;
        }
        // 相信已经翻转除头部外的所有节点为last，
        // 连接last和原头部，原头部指向null
        // 返回翻转后的头部last
        ListNode last = reverseList(head.next);
        head.next.next = head;
        head.next = null;
        return last;
    }
}
```
Continue...









