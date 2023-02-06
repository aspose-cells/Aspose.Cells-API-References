---
title: exclude_unused_styles property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 130
url: /python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles/
is_root: false
---

## exclude_unused_styles property


Indicating whether excludes unused styles.
For the generated html files, excluding unused styles can make the file size smaller
without affecting the visual effects. So the default value of this property is true.
If user needs to keep all styles in the workbook for the generated html(such as the scenario that user
needs to restore the workbook from the generated html later), please set this property as false.
### Definition:
```python
@property
def exclude_unused_styles(self):
    ...
@exclude_unused_styles.setter
def exclude_unused_styles(self, value):
    ...
```

### See Also
* module [aspose.cells](../../)
* class [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions)
