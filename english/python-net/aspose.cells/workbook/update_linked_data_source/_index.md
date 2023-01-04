---
title: update_linked_data_source method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 410
url: /python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---

## update_linked_data_source(external_workbooks) {#list}

If this workbook contains external links to other data source,
Aspose.Cells will attempt to retrieve the latest data.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| external_workbooks | list | External workbooks are referenced by this workbook.<br/>If it's null, we will directly open the external linked files..<br/>If it's not null, <br/>we will check whether the external link in the array first;<br/>if not, we will open the external linked files again. |
### Remarks

If the method is not called before calculating formulas,
Aspose.Cells will use the previous information(cached in the file);
Please set CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath. 
And please set Workbook.FilePath if this workbook is from a stream,
otherwise Aspose.Cells could not get the external link full path sometimes.


### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)
