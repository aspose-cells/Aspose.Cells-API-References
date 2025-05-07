---
title: PowerQueryFormulaItem.Value
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaItem property. Gets the value of the item
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitem/value/
---
## PowerQueryFormulaItem.Value property

Gets the value of the item.

```csharp
public string Value { get; set; }
```

### Examples

```csharp
// Called: item.Value = item.Value.Replace(@"\\bud-fs\sed corp\sales\", @"\\aspose.com\data\sales\");
[Test]
        public void Property_Value()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet48061.xlsx");
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula f in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
                {
                    if (item.Name == "Source")
                    {
                        Console.WriteLine("Original Source: " + item.Value);
                        item.Value = item.Value.Replace(@"\\bud-fs\sed corp\sales\", @"\\aspose.com\data\sales\");
                        Console.WriteLine("New Source: " + item.Value);

                    }
                }
            }
            workbook.Save(Constants.destPath + "CellsNet48061.xlsx");
        }
```

### See Also

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


