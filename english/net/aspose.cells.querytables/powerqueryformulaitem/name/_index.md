---
title: PowerQueryFormulaItem.Name
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaItem property. Gets the name of the item
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitem/name/
---
## PowerQueryFormulaItem.Name property

Gets the name of the item.

```csharp
public string Name { get; }
```

### Examples

```csharp
// Called: Console.Write(item.Name + &amp;quot; = &amp;quot;);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46924.xlsx&quot;);
            DataMashup mashupData = workbook.DataMashup;
            Assert.AreEqual(3, mashupData.PowerQueryFormulas.Count);
            foreach (PowerQueryFormula f in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
                foreach (PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
                {
                    Console.Write(item.Name + &quot; = &quot;);
                    Console.WriteLine(item.Value);
                }
            }
            workbook.Save(Constants.destPath + &quot;CellsNet46924.xlsx&quot;);
        }
```

### See Also

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


