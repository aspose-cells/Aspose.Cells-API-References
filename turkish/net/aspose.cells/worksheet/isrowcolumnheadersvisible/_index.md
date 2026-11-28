---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten değeri alır veya ayarlar. Varsayılan değer true'tır."
type: docs
url: /tr/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten değeri alır veya ayarlar. Varsayılan değer true'tur.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır ve sütun başlıklarının görünürlüğünü false olarak ayarla
            worksheet.IsRowColumnHeadersVisible = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyerek özelliği doğrulayın
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Özellik değerini çıktı olarak ver
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


