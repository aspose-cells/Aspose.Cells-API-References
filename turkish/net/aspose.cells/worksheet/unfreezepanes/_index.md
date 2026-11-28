---
title: "Worksheet.UnFreezePanes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Çalışma sayfasındaki bölmeleri serbest bırakır"
type: docs
url: /tr/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Çalışma sayfasındaki bölmeleri dondurmayı kaldırır.

```csharp
public void UnFreezePanes()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // C3 hücresinde bölmeleri dondur (2. satır, 2. sütun donduruldu)
            worksheet.FreezePanes("C3", 2, 2);

            // Bölmelerin dondurulduğunu doğrula
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Bölmelerin dondurulmasını kaldır
            worksheet.UnFreezePanes();

            // Bölmelerin dondurulmadığını doğrula
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Çalışma kitabını kaydedin
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


