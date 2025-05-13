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
public void PowerQueryFormula_Property_Name()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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
    workbook.Save(Constants.destPath + "example.xlsx");
    Util.SaveForViewer(workbook, "13", "example.xls");
}
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


