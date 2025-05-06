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
// Called: Assert.AreEqual(&amp;quot;Klant Analyse/Outsystems Exports/Helper Queries&amp;quot;, queries[0].GroupName);
[Test]
        public void Property_GroupName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET57738.xlsx&quot;);
            var queries = workbook.DataMashup.PowerQueryFormulas;
           Assert.AreEqual(&quot;Klant Analyse/Outsystems Exports/Helper Queries&quot;,queries[0].GroupName);
            workbook.Save(Constants.destPath + &quot;CELLSNET57738.xlsx&quot;);
             workbook = new Workbook(Constants.destPath + &quot;CELLSNET57738.xlsx&quot;);
             queries = workbook.DataMashup.PowerQueryFormulas;
            Assert.AreEqual(&quot;Klant Analyse/Outsystems Exports/Helper Queries&quot;, queries[0].GroupName);
        }
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


