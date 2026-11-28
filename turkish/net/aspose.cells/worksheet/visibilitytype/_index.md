---
title: "Worksheet.VisibilityType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu sayfa için görünür durumu gösterir"
type: docs
url: /tr/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Bu sayfanın görünür durumunu gösterir.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfaları ekle
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Her çalışma sayfası için farklı görünürlük türlerini ayarla
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // Çalışma kitabını kaydedin
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // Görünürlük ayarlarını doğrulamak için çalışma kitabını yeniden yükle
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Görünürlük türlerini çıktı olarak ver
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


