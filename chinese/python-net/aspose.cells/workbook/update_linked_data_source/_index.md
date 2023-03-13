---
title: update_linked_data_source方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 410
url: /zh/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
如果此工作簿包含指向其他数据源的外部链接，
Aspose.Cells 将尝试检索最新数据。



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| external_workbooks | list |此工作簿引用外部工作簿。<br/>如果为空，我们将直接打开外部链接文件。<br/>如果它不为空，<br/>我们会先检查数组中是否有外部链接；<br/>如果没有，我们将重新打开外部链接文件。|
### 评论

如果在计算公式之前未调用该方法，
Aspose.Cells 将使用以前的信息（缓存在文件中）；
请设置 CellsHelper.StartupPath、CellsHelper.AltStartPath、CellsHelper.LibraryPath。
如果此工作簿来自流，请设置 Workbook.FilePath，
否则 Aspose.Cells 有时无法获取外部链接的完整路径。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
