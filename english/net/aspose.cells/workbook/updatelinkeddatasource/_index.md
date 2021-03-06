---
title: UpdateLinkedDataSource
second_title: Aspose.Cells for .NET API Reference
description: If this workbook contains external links to other data source Aspose.Cells will attempt to retrieve the latest data.
type: docs
weight: 680
url: /net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | External workbooks are referenced by this workbook. If it's null, we will directly open the external linked files.. If it's not null, we will check whether the external link in the array first; if not, we will open the external linked files again. |

### Remarks

If the method is not called before calculating formulas, Aspose.Cells will use the previous information(cached in the file); Please set CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath. And please set Workbook.FilePath if this workbook is from a stream, otherwise Aspose.Cells could not get the external link full path sometimes.

### See Also

* class [Workbook](../../workbook)
* namespace [Aspose.Cells](../../workbook)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
