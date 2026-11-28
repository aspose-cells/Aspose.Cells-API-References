---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Elektronik tablo açıldığında etkin çalışma sayfasının dizinini temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Elektronik tablo açıldığında etkin çalışma sayfasının dizinini temsil eder.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Açıklamalar

Sayfa indeksi sıfır tabanlıdır.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // 3 çalışma sayfası içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Etkin sayfa indeksini 1 olarak ayarla (ikinci sayfa)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Etkin sayfayı doğrula
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // Çalışma kitabını kaydedin
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


