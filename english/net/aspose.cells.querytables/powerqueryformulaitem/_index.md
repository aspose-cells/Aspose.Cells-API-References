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
// Called: foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
[Test]
        public void Type_PowerQueryFormulaItem()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet48061.xlsx&quot;);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula f in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
                {
                    if (item.Name == &quot;Source&quot;)
                    {
                        Console.WriteLine(&quot;Original Source: &quot; + item.Value);
                        item.Value = item.Value.Replace(@&quot;\\bud-fs\sed corp\sales\&quot;, @&quot;\\aspose.com\data\sales\&quot;);
                        Console.WriteLine(&quot;New Source: &quot; + item.Value);

                    }
                }
            }
            workbook.Save(Constants.destPath + &quot;CellsNet48061.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


