---
title: DataMashup.PowerQueryFormulas
second_title: Aspose.Cells for .NET API Reference
description: DataMashup property. Gets all power query formulas
type: docs
url: /net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Gets all power query formulas.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Examples

```csharp
// Called: foreach (PowerQueryFormula f in mashupData.PowerQueryFormulas)
public void DataMashup_Property_PowerQueryFormulas()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");

    DataMashup mashupData = workbook.DataMashup;
            
    Assert.AreEqual("Timesheets", mashupData.PowerQueryFormulas[0].Name);
    Assert.AreEqual("PQVLookUp", mashupData.PowerQueryFormulas[1].Name);
    Assert.AreEqual("tPeriodTable", mashupData.PowerQueryFormulas[2].Name);
    workbook.Save(Constants.destPath + "example.xlsm");

    workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    mashupData = workbook.DataMashup;
    foreach (PowerQueryFormula f in mashupData.PowerQueryFormulas)
    {
        Console.WriteLine(f.Name);
    }
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


