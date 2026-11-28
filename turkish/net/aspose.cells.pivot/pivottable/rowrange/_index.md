---
title: "PivotTable.RowRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. PivotTable raporundaki satır alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

PivotTable raporundaki satır alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur.

```csharp
public CellArea RowRange { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // Çalışma kitabındaki tüm pivot tablolarını yenile
            workbook.Worksheets.RefreshAll();
            
            // İlk çalışma sayfasındaki ilk pivot tabloyu alın
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // Pivot tablonun satır aralığını alın
            CellArea rowRange = pivotTable.RowRange;
            
            // Satır aralığı koordinatlarını gösterin
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // Pivot tablonun sütun aralığını alın
            CellArea columnRange = pivotTable.ColumnRange;
            
            // Sütun aralığı koordinatlarını gösterin
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


