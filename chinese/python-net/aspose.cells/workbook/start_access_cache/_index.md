---
title: start_access_cache方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 380
url: /zh/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
启动使用缓存访问数据的会话。



```python
def start_access_cache(self, opts):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/zh/python-net/aspose.cells/accesscacheoptions) |数据访问选项|
### 评论

如果指定数据访问的缓存要求工作表中的某些数据模型为“只读”，
那么这个工作簿中每个工作表中对应的数据模型将被视为“只读”
并且用户不应更改其中任何一个。


完成对数据的访问后，[Workbook.close_access_cache(opts)](/cells/zh/python-net/aspose.cells/workbook/close_access_cache)应该
使用相同的选项调用以清除所有缓存并恢复正常访问模式。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
