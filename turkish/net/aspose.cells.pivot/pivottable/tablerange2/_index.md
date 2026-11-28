---
title: "PivotTable.TableRange2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Tüm PivotTable raporunu ve sayfa alanlarını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Tüm PivotTable raporunu ve sayfa alanlarını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur.

```csharp
public CellArea TableRange2 { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange2Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Bir pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Verileri hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Tüm pivot tabloyu içeren TableRange2'yi alın
            CellArea tableRange2 = pivotTable.TableRange2;
            Console.WriteLine($"TableRange2: StartRow={tableRange2.StartRow}, StartColumn={tableRange2.StartColumn}, " +
                $"EndRow={tableRange2.EndRow}, EndColumn={tableRange2.EndColumn}");

            // TableRange2'ye dayalı bir aralık oluşturun
            Aspose.Cells.Range pivotRange = worksheet.Cells.CreateRange(
                tableRange2.StartRow, 
                tableRange2.StartColumn, 
                tableRange2.EndRow - tableRange2.StartRow + 1, 
                tableRange2.EndColumn - tableRange2.StartColumn + 1);

            // Aralık adresini çıktı olarak ver
            Console.WriteLine($"Pivot Table Range: {pivotRange.Address}");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


