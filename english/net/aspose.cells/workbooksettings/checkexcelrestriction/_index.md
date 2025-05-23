---
title: WorkbookSettings.CheckExcelRestriction
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValuestring if this property is true you will get an Exception. If this property is false we will accept your input string value as the cells value so that later you can output the complete string value for other file formats such as CSV. However if you have set such kind of value that is invalid for excel file format you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file
type: docs
url: /net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.CheckExcelRestriction = false;
public void WorkbookSettings_Property_CheckExcelRestriction()
{
    Workbook workbook = new Workbook();
    workbook.Settings.CheckExcelRestriction = false;
    workbook.Worksheets[0].Cells["A1"].PutValue(new string('a', 40000));
    workbook = Util.ReSave(workbook, new TxtSaveOptions(),
        new TxtLoadOptions() { CheckDataValid = false, CheckExcelRestriction = false });
    Assert.AreEqual(40000, workbook.Worksheets[0].Cells["A1"].StringValue.Length, "Long string exceeds liimit");
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


