---
title: PowerQueryFormula.Name
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets and sets the name of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Gets and sets the name of the power query formula.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(f.Name);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet57297.xlsx&quot;);
            foreach (PowerQueryFormula f in workbook.DataMashup.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
            }
            Assert.AreEqual(&quot;ProcessWorksheetTemplate&quot;, workbook.DataMashup.PowerQueryFormulas[0].Name);
            workbook.Save(Constants.destPath + &quot;CellsNet57297.xlsx&quot;);


        }
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


