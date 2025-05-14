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
// Called: if (item.Name == "Source")
public void PowerQueryFormulaItem_Property_Name()
{

    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


