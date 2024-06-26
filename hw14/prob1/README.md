# 第 14 次作业: 第 1 题

## 验证部分

### 测试思路

为了确保 `U_DoubleLongLong` 这一共用体的功能能够正常工作，我设计了以下测试样例：

1. 测试 $2$​ 的正整数次幂
   输入 $2147483648$，输出为
   ```
   2.14748e+09 is stored as 0100000111100000000000000000000000000000000000000000000000000000.
   ```
2. 测试 $2$​ 的负整数次幂
   输入 $0.125$，输出为
   ```
   0.125 is stored as 0011111111000000000000000000000000000000000000000000000000000000.
   ```
3. 测试 $0$​
   输入 $0$，输出为
   ```
   0 is stored as 0000000000000000000000000000000000000000000000000000000000000000.
   ```
4. 测试负数
   输入 $-4$，输出为
   ```
   -4 is stored as 1100000000010000000000000000000000000000000000000000000000000000.
   ```
5. 测试其他数
   输入 $1234567.1234567$，输出为
   ```
   1.23457e+06 is stored as 0100000100110010110101101000011100011111100110101101101110111001.
   ```
6. 测试“非数”
   运行得到结果：
   ```
   nan is stored as 1111111111111000000000000000000000000000000000000000000000000000.
   ```

通过手工计算，同时查询[浮点数-Float-Double转二进制 - ToolTT在线工具箱](https://tooltt.com/floatconverter/)，可以发现以上输出均符合预期，因此全部测试均通过。

## 如何进行测试

最后得到可执行文件`CP_UnionDoubleLongLongMain.exe`。运行该可执行文件后按照提示进行输入，观察输出和预期是否相同。

## 如何编译及运行

在 `hw14/prob1/UnionDoubleLongLong/` 目录下，执行

```
g++ CP_UnionDoubleLongLong.cpp CP_UnionDoubleLongLongMain.cpp -o CP_UnionDoubleLongLongMain.exe
```

即可编译得到可执行文件 `CP_UnionDoubleLongLongMain.exe`。运行该可执行文件后按照提示进行输入。
