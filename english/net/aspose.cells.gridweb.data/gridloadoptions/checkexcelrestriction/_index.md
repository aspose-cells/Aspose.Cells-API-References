---
title: GridLoadOptions.CheckExcelRestriction
second_title: Aspose.Cells for .NET API Reference
description: GridLoadOptions property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValuestring if this property is true you will get an Exception. If this property is false we will accept your input string value as the cells value so that later you can output the complete string value for other file formats such as CSV. However if you have set such kind of value that is invalid for excel file format you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file
type: docs
url: /net/aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/
---
## GridLoadOptions.CheckExcelRestriction property

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### See Also

* class [GridLoadOptions](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


