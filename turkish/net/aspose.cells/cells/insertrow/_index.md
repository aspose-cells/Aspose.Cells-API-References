---
title: "Cells.InsertRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Çalışma sayfasına yeni bir satır ekler"
type: docs
url: /tr/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Çalışma sayfasına yeni bir satır ekler.

```csharp
public void InsertRow(int rowIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hücre koleksiyonunu al
            Cells cells = sheet.Cells;
            
            // Satır 6'ya örnek veri ekleyin
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // Satır 7'ye örnek veri ekleyin
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // İndeks 7'de yeni bir satır ekleyin (mevcut satır 7'yi aşağı kaydırır)
            cells.InsertRow(7);
            
            // Yeni eklenen satıra veri ekleyin
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // Çalışma kitabını kaydedin
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


