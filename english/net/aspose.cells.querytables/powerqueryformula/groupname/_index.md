---
title: PowerQueryFormula.GroupName
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets the name of group which contains this power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/groupname/
---
## PowerQueryFormula.GroupName property

Gets the name of group which contains this power query formula.

```csharp
public string GroupName { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Klant Analyse/Outsystems Exports/Helper Queries",queries[0].GroupName);
public void PowerQueryFormula_Property_GroupName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var queries = workbook.DataMashup.PowerQueryFormulas;
   Assert.AreEqual("Klant Analyse/Outsystems Exports/Helper Queries",queries[0].GroupName);
    workbook.Save(Constants.destPath + "example.xlsx");
     workbook = new Workbook(Constants.destPath + "example.xlsx");
     queries = workbook.DataMashup.PowerQueryFormulas;
    Assert.AreEqual("Klant Analyse/Outsystems Exports/Helper Queries", queries[0].GroupName);
}
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


