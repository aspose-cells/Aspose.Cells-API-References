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
[Test]
        public void Property_RefreshDate()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46394_&quot;;
            Workbook wb = new Workbook(filePath + &quot;Sample.xlsx&quot;);
            PivotTable pt = wb.Worksheets[0].PivotTables[0];
            Console.WriteLine(pt.RefreshDate.ToUniversalTime());
            Console.WriteLine(pt.RefreshedByWho);

            string savePath = CreateFolder(filePath);
            wb.Save(savePath + &quot;out.xlsb&quot;);
            wb.Save(savePath + &quot;out.xls&quot;);
            wb.Save(savePath + &quot;out.xlsx&quot;);
            wb = new Workbook(savePath + &quot;out.xlsx&quot;);
            pt = wb.Worksheets[0].PivotTables[0];
            Console.WriteLine(pt.RefreshDate.ToLongDateString());
            Console.WriteLine(pt.RefreshedByWho);
            wb = new Workbook(savePath + &quot;out.xlsb&quot;);
            pt = wb.Worksheets[0].PivotTables[0];
            Console.WriteLine(pt.RefreshDate.ToLongDateString());
            Console.WriteLine(pt.RefreshedByWho);
            wb = new Workbook(savePath + &quot;out.xls&quot;);
            pt = wb.Worksheets[0].PivotTables[0];
            Console.WriteLine(pt.RefreshDate.ToLongDateString());
            Console.WriteLine(pt.RefreshedByWho);
            Console.WriteLine(&quot;========================\n&quot;);

            wb = new Workbook(filePath + &quot;Sample.xlsb&quot;);
            pt = wb.Worksheets[0].PivotTables[0];
            Console.WriteLine(pt.RefreshDate.ToLongDateString());
            Console.WriteLine(pt.RefreshedByWho);

            wb = new Workbook(filePath + &quot;Sample.xls&quot;);
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


