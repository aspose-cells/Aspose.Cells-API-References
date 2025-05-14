---
title: LoadOptions.CheckExcelRestriction
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValuestring if this property is true you will get an Exception. If this property is false we will accept your input string value as the cells value so that later you can output the complete string value for other file formats such as CSV. However if you have set such kind of value that is invalid for excel file format you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file
type: docs
url: /net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Examples

```csharp
// Called: loadOptions.CheckExcelRestriction = false;
public void LoadOptions_Property_CheckExcelRestriction()
{
    Workbook wb = new Workbook();
    Workbook workbook = new Workbook();
    workbook.Settings.CheckExcelRestriction = false;

    Worksheet worksheet = workbook.Worksheets[0];
    Cells cells = worksheet.Cells;
    string str = Repeat("x",32767) + " Testing if it works or not";
    cells["A1"].PutValue(str);
    Assert.AreEqual(str, cells["A1"].StringValue);
          

    OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
    saveOptions.CheckExcelRestriction = false;

    workbook.Save(Constants.destPath + "example.xlsx", saveOptions);

    LoadOptions loadOptions = new LoadOptions();
    loadOptions.CheckExcelRestriction = false;
    workbook = new Workbook(Constants.destPath + "example.xlsx", loadOptions);
    Assert.AreEqual(str, workbook.Worksheets[0].Cells["A1"].StringValue);
    Assert.IsTrue(workbook.Worksheets[0].Cells["A1"].StringValue.Length > short.MaxValue);
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


