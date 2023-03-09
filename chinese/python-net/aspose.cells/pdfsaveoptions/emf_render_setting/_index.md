---
title: emf_render_setting 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 200
url: /zh/python-net/aspose.cells/pdfsaveoptions/emf_render_setting/
is_root: false
---
## emf_render_setting 属性

渲染 Emf 图元文件的设置。

### 评论

标识为“EMF+ Dual”的 EMF 图元文件可以包含 EMF+ 记录和 EMF 记录。
任何一种记录都可以用来渲染图像，只有 EMF+ 条记录，或者只有 EMF 条记录。
当设置[EmfRenderSetting.EMF_PLUS_PREFER](/cells/zh/python-net/aspose.cells/emfrendersetting#EMF_PLUS_PREFER)时，那么在渲染成pdf时会解析EMF+条记录，否则只解析EMF条记录。
默认值为 [EmfRenderSetting.EMF_ONLY](/cells/zh/python-net/aspose.cells/emfrendersetting#EMF_ONLY)。
### 定义：
```python
@property
def emf_render_setting(self):
    ...
@emf_render_setting.setter
def emf_render_setting(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [EmfRenderSetting](/cells/zh/python-net/aspose.cells/emfrendersetting)
* 类 [PdfSaveOptions](/cells/zh/python-net/aspose.cells/pdfsaveoptions)
