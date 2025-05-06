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
// Called: item.Value = item.Value.Replace(@&amp;quot;vente&amp;quot;, @&amp;quot;aspose&amp;quot;);
[Test]
        public void Property_Value()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Cells48460.xlsm&quot;);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula f in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in f.PowerQueryFormulaItems)
                {
                    if (item.Name == &quot;Source&quot;)
                    {
                        Console.WriteLine(&quot;Original Source: &quot; + item.Value);
                        item.Value = item.Value.Replace(@&quot;vente&quot;, @&quot;aspose&quot;);
                        Console.WriteLine(&quot;New Source: &quot; + item.Value);
                    }
                }
            }
            workbook.Save(Constants.destPath + &quot;Cells48460.xlsx&quot;);
            //   workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


