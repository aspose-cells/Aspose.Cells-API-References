---
title: export_object method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/iexportobjectlistener/export_object/
is_root: false
---

## export_object(e) {#ExportObjectEvent}

Export one object.

### Returns 


The information about the result of exporting object.

* For exporting objects when export workbook to HTML format,
the result is URL string to access the saved Image from the html file which contains this exported object.


```python
def export_object(self, e):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| e | [ExportObjectEvent](/cells/python-net/aspose.cells/exportobjectevent) | The event triggered when one object needs to be exported. |



### See Also
* module [aspose.cells](../../)
* class [IExportObjectListener](/cells/python-net/aspose.cells/iexportobjectlistener)
