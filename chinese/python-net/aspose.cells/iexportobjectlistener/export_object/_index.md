---
title: export_object方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/iexportobjectlistener/export_object/
is_root: false
---
##  export_object(e) {#ExportObjectEvent}
导出一个对象。


### 返回

导出对象的结果信息。

* 用于将工作簿导出为 HTML 格式时导出对象，
结果是 URL 字符串，用于从包含此导出对象的 html 文件访问保存的图像。


```python
def export_object(self, e):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| e | [ExportObjectEvent](/cells/zh/python-net/aspose.cells/exportobjectevent) |当需要导出一个对象时触发的事件。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [IExportObjectListener](/cells/zh/python-net/aspose.cells/iexportobjectlistener)
