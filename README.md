# Tricky_4803_Tree

made by Jaehyeok Choi

## Welcome to Jaehyeok's github!

## What is the problem?

![image](https://github.com/Choi-JaeHyeok-21500749/Tricky_4803_Tree/blob/main/4803_pro.PNG)

## What Algorithm should I use?

Graph Algorithm , union-find

## What was the key point and the hard part?

It was tricky one I think.

Because at first , I though if I detect a cycle(find(x) == find(y)) then , does not count the root of them will work.

However , It was wrong. 

For example,

Let's say there is a cycle in node 1, 2 ,3 and find(1) == find(2) == find(3) == 1.

In thie case we add (1,4) , it will think there is one tree bacause node 1 and node 4 is not connected before.

In fact, because we have a cylce in node 1, 2,3,4, the answer should be No tree.

So, by adding check array , If check[find(x)] or check[find(y)] is checked (true) I make find(x) checked.

After these sequences , search (1 ~ N)'s root and if that value is not checked, increase the number of thee(s).

## Where can I get more help, if I need it?

You can contact me through email, which is wogur7496@gmail.com.
Thank you for visiting this github!
