---
title: ListColumn.GetCustomCalculatedFormula
second_title: Aspose.Cells for .NET API Reference
description: ListColumn method. Gets the formula of this list column
type: docs
url: /net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

Gets the formula of this list column.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Return Value

The formula of this list column.

### Examples

```csharp
// Called: listObject.ListColumns[2].GetCustomCalculatedFormula(false, false), "CalculatedFormula");
public void ListColumn_Method_GetCustomCalculatedFormula()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = wb.Worksheets["DataSource"];
    ListObject listObject = sheet.ListObjects["UserReport_2_Table_1"];
    for (int i = 0; i < listObject.ListColumns.Count; i++)
    {
        ListColumn listColumn = listObject.ListColumns[i];
        listColumn.Name = "UserColumn" + i;
    }
    Assert.AreEqual("=WEEKNUM([@UserColumn1])",
        listObject.ListColumns[2].GetCustomCalculatedFormula(false, false), "CalculatedFormula");
}
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


