---
title: PivotTable.RefreshDate
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the last date time when the PivotTable was refreshed
type: docs
url: /net/aspose.cells.pivot/pivottable/refreshdate/
---
## PivotTable.RefreshDate property

Gets the last date time when the PivotTable was refreshed.

```csharp
public DateTime RefreshDate { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(pt.RefreshDate.ToLongDateString());
public void PivotTable_Property_RefreshDate()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46394_";
    Workbook wb = new Workbook(filePath + "Sample.xlsx");
    PivotTable pt = wb.Worksheets[0].PivotTables[0];
    Console.WriteLine(pt.RefreshDate.ToUniversalTime());
    Console.WriteLine(pt.RefreshedByWho);

    string savePath = CreateFolder(filePath);
    wb.Save(savePath + "out.xlsb");
    wb.Save(savePath + "out.xls");
    wb.Save(savePath + "out.xlsx");
    wb = new Workbook(savePath + "out.xlsx");
    pt = wb.Worksheets[0].PivotTables[0];
    Console.WriteLine(pt.RefreshDate.ToLongDateString());
    Console.WriteLine(pt.RefreshedByWho);
    wb = new Workbook(savePath + "out.xlsb");
    pt = wb.Worksheets[0].PivotTables[0];
    Console.WriteLine(pt.RefreshDate.ToLongDateString());
    Console.WriteLine(pt.RefreshedByWho);
    wb = new Workbook(savePath + "out.xls");
    pt = wb.Worksheets[0].PivotTables[0];
    Console.WriteLine(pt.RefreshDate.ToLongDateString());
    Console.WriteLine(pt.RefreshedByWho);
    Console.WriteLine("========================\n");

    wb = new Workbook(filePath + "Sample.xlsb");
    pt = wb.Worksheets[0].PivotTables[0];
    Console.WriteLine(pt.RefreshDate.ToLongDateString());
    Console.WriteLine(pt.RefreshedByWho);

    wb = new Workbook(filePath + "Sample.xls");
    pt = wb.Worksheets[0].PivotTables[0];
    Console.WriteLine(pt.RefreshDate.ToLongDateString());
    Console.WriteLine(pt.RefreshDate.ToLongDateString());
    Console.WriteLine(pt.RefreshedByWho);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


