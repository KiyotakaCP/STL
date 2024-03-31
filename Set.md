# Set

### 把元素 x 加進 set
```cpp
st.insert(x);
```

### 檢查元素 x 是否存在 set 中
```cpp
st.count(x);
```

### 刪除元素 x
```cpp
st.erase(x); // 可傳入值或iterator
```

### 取值：使用iterator
```cpp
x = *st.begin(); // set 中的第一個元素(最小的元素)
x = *st.rbegin(); // set 中的最後一個元素(最大的元素)
```

### Binary Search
```cpp
auto it = st.find(x); // binary search, O(log(N))
auto it = st.lower_bound(x); // binary search, O(log(N))
auto it = st.upper_bound(x); // binary search, O(log(N))
```

## Multiset
```cpp
st.erase(val); // 會刪除所有值為 val 的元素
st.erase(st.find(val)); // 只刪除第一個值為 val 的元素
```