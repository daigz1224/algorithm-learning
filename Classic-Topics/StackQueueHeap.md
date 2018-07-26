# Stack Queue Heap

## 经典题

### 使用队列实现栈

- [225. Implement Stack using Queues](https://leetcode.com/problems/implement-stack-using-queues/description/)

### 使用栈实现队列

- [232. Implement Queue using Stacks](https://leetcode.com/problems/implement-queue-using-stacks/description/)

### 包含min函数的栈

- [155. Min Stack](https://leetcode.com/problems/min-stack/description/)

### 合法的出栈序列

- poj 1363 Rails

```c++
bool check_is_valid_order (std::queue<int> &order) {
    std::stack<int> S;
    int n = order.size();
    for (int i = 1; i <= n; i++) {
        S.push(i);
        while (!S.empty() && order.front() == S.top()) {
            S.pop();
            order.pop();
        }
   }
   if (!S.empty())
       return false;
      return true;
}
```

### 简单的计算器（栈）

- [224. Basic Calculator](https://leetcode.com/problems/basic-calculator/description/)

### 数组中第K大的数（堆）

- [215. Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/description/)

### 寻找中位数（堆）

- [295. Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream/description/)