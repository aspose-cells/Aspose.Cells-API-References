---
title: set_embedded_object method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 170
url: /python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---

## set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}

Sets embedded object data.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| link_to_file | bool | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| object_data | bytes | The embedded object data. |
| source_file_name | str | The file name. |
| display_as_icon | bool | Indicates whether diplaying object as an icon.<br/>If true, the orginal image data will be covered by icon. |
| label | str | The icon label. Only works when displayAsIcon as true. |


## set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}

Sets embedded object data.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| link_to_file | bool | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| object_data | bytes | The embedded object data. |
| source_file_name | str | The file name. |
| display_as_icon | bool | Indicates whether diplaying object as an icon.<br/>If true, the orginal image data will be covered by icon. |
| label | str | The icon label. Only works when displayAsIcon as true. |
| update_icon | bool | Indicates whether automatically updating icon. |
### Remarks

As Aspose can update embedd all file icons, so it's better that you can add correct icon with `update_icon` as false.


### See Also
* module [aspose.cells.drawing](../../)
* class [OleObject](/cells/python-net/aspose.cells.drawing/oleobject)
