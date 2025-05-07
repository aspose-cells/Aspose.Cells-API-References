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
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet52612.xlsx");
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula f in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
                {
                    //if (item.Name == "Source")
                    //{
                    Console.WriteLine("Original Source: " + item.Value);
                    item.Value = item.Value.Replace(@"Central", @"OLIVER");
                    Console.WriteLine("New Source: " + item.Value);

                    //}
                }
            }
            workbook.Save(Constants.destPath + "CellsNet52612.xlsx");
            Util.SaveForViewer(workbook, "13", "CellsNet52612.xls");
        }
```

### See Also

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


