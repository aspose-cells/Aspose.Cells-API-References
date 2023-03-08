---
title: multi_thread_reading 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1200
url: /zh/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
## multi_thread_reading 属性

获取或设置单元格数据模型是否应支持多线程读取。
此属性的默认值为 false。

### 评论

如果有多个线程同时读取这个集合中的Row/Cell对象，
此属性应设置为 true，否则可能会产生意想不到的结果。
支持多线程读取可能会降低从该集合访问 Row/Cell 对象的性能。
请注意，部分功能不支持多线程读取，
例如格式化值（按 [Cell.string_value](/cells/zh/python-net/aspose.cells/cell#string_value)、[Cell.display_string_value](/cells/zh/python-net/aspose.cells/cell#display_string_value) 等）。
因此，即使将此属性设置为 true，这些 API 仍然可能为多线程读取提供意想不到的结果。
### 定义：
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
