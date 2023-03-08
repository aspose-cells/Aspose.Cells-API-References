---
title: on_circular方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
在计算循环引用的公式时实现这个方法来做业务。


### 返回

调用后公式引擎是否需要循环计算这些单元格。
真正让公式引擎继续为他们做计算。
False 让公式引擎只将这些单元格标记为已计算。


```python
def on_circular(self, circular_cells_data):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator |带有 CalculationCell 项的 IEnumerator 表示单元格<br/>依赖于循环引用。|
### 评论

在实现中用户也可以将期望值设置为计算结果
对于部分/所有这些单元格，因此公式引擎不会递归计算它们。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [AbstractCalculationMonitor](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor)
