---
title: Class PowerQueryFormulaItem
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormulaItem class. Represents the item of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Represents the item of the power query formula.

```csharp
public class PowerQueryFormulaItem
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Gets the name of the item. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Gets the value of the item. |

### Examples

```csharp
// Called: PowerQueryFormulaItem PQFI = PQFIcoll[0];
public void QueryTables_Type_PowerQueryFormulaItem()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");

    PowerQueryFormulaCollection PQFcoll = workbook.DataMashup.PowerQueryFormulas;//Exception here
    Assert.AreEqual(PQFcoll.Count, 2);

    PowerQueryFormula PQF = PQFcoll[1];
    Assert.AreEqual("Change Management", PQF.Name);
    PowerQueryFormulaItemCollection PQFIcoll = PQF.PowerQueryFormulaItems;
    Assert.AreEqual(3, PQFIcoll.Count);

    PowerQueryFormulaItem PQFI = PQFIcoll[0];
    Assert.AreEqual("Source", PQFI.Name);
    Assert.AreEqual(PQFI.Value, "SharePoint.Tables(\"https://cimconuso.sharepoint.com\", [ApiVersion = 15])");

    workbook.Save(Constants.destPath + "example.xlsm");

}
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


