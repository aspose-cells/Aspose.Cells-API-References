---
title: CellsHelper.GetVersion
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Get the release version
type: docs
url: /net/aspose.cells/cellshelper/getversion/
---
## CellsHelper.GetVersion method

Get the release version.

```csharp
public static string GetVersion()
```

### Return Value

The release version.

### Examples

```csharp
// Called: Console.WriteLine(CellsHelper.GetVersion());
public void CellsHelper_Method_GetVersion()
{
    Console.WriteLine(CellsHelper.GetVersion());
    if (2 == 1)
    {
        long t = DateTime.Now.ToFileTimeUtc();
        Console.WriteLine("Loading...");
        Workbook wb = new Workbook("example.xlsx");
        Console.WriteLine(DateTime.Now.ToFileTimeUtc() - t);
        t = DateTime.Now.ToFileTimeUtc();
        Worksheet sheet = wb.Worksheets[0];
        Cells cells = sheet.Cells;
        Console.WriteLine("Finished. Calculating...");
        wb.CalculateFormula();
        Console.WriteLine(DateTime.Now.ToFileTimeUtc() - t);
        //Util.ReSave(wb, SaveFormat.Xlsb);
    }
}
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


