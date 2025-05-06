---
title: PowerQueryFormula.PowerQueryFormulaItems
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets all items of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Gets all items of power query formula.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Examples

```csharp
// Called: foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
[Test]
        public void Property_PowerQueryFormulaItems()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet52612.xlsx&quot;);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula f in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
                {
                    //if (item.Name == &quot;Source&quot;)
                    //{
                    Console.WriteLine(&quot;Original Source: &quot; + item.Value);
                    item.Value = item.Value.Replace(@&quot;Central&quot;, @&quot;OLIVER&quot;);
                    Console.WriteLine(&quot;New Source: &quot; + item.Value);

                    //}
                }
            }
            workbook.Save(Constants.destPath + &quot;CellsNet52612.xlsx&quot;);
            Util.SaveForViewer(workbook, &quot;13&quot;, &quot;CellsNet52612.xls&quot;);
        }
```

### See Also

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


