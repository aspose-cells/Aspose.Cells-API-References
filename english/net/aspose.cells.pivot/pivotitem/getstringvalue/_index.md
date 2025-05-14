---
title: PivotItem.GetStringValue
second_title: Aspose.Cells for .NET API Reference
description: PivotItem method. Gets the string value of the pivot item If the value is null it will return 
type: docs
url: /net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Gets the string value of the pivot item If the value is null, it will return ""

```csharp
public string GetStringValue()
```

### Examples

```csharp
// Called: Assert.IsTrue(pf.PivotItems[1].GetStringValue().IndexOf("4:48:00") != -1);
public void PivotItem_Method_GetStringValue()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsb");
    PivotField pf = workbook.Worksheets[0].PivotTables[0].RowFields[0];
   Assert.IsTrue(pf.PivotItems[1].GetStringValue().IndexOf("4:48:00") != -1);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsb");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsb");
    pf = workbook.Worksheets[0].PivotTables[0].RowFields[0];
    Assert.IsTrue(pf.PivotItems[1].GetStringValue().IndexOf("4:48:00") != -1);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    pf = workbook.Worksheets[0].PivotTables[0].RowFields[0];
    Assert.IsTrue(pf.PivotItems[1].GetStringValue().IndexOf("4:48:00") != -1);
}
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


