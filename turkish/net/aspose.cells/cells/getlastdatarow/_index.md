---
title: "Cells.GetLastDataRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen sütunda veri içeren son hücrenin satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Belirtilen sütunda veri içeren hücrenin son satır indeksini alır.

```csharp
public int GetLastDataRow(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

son satır indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // A sütunundaki (indeks 0) son veri satırını al
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // Son veri satırından sonra yeni bir satır ekle
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // Yeni satıra veri ekle
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


