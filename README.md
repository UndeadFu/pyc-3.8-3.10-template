# pyc-3.8-3.10-template



### 0x00 说明

010 Editor 中的 pyc.bt 是 python 2.x 版本的，不能解析 python 3.x 的。
由于 pyc 在 3.8 版本做了一点结构上的调整，因此本项目暂时不支持 3.7 及以下的解析。
后续有机会再做修复。



### 0x01 当前的 bug 和预计修复日期

由于是业余搞的，排期比较拖沓。

1. 解析数据时，对 TYPE_LONG, TYPE_BINARY_FLOAT, TYPE_COMPLEX, TYPE_BINARY_COMPLEX 没有做处理，会导致后续结构出错。 预计 6 月中旬修复
2. 对于 python 版本的判断做得粗糙。预计 7 月修复
3. 头部跳过了 4 个字节。预计 7 月修复
4. 指令未解析。预计 7 月修复
5. FLAG_REF 的意义暂时不清晰，没有解析。预计 8 月修复
6. 更多版本的支持待定