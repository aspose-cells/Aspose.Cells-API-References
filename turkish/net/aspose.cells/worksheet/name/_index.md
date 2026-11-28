---
title: "Worksheet.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasının adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Çalışma sayfasının adını alır veya ayarlar.

```csharp
public string Name { get; set; }
```

### Açıklamalar

Sayfa adının maksimum uzunluğu 31'dir. Ve iki çalışma sayfasına aynı adı (büyük/küçük harfe duyarsız) atayamazsınız. Örneğin, "SheetName1" adını ilk çalışma sayfasına ayarlayamaz ve "SHEETNAME1" adını ikinci çalışma sayfasına ayarlayamazsınız.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına erişin ve adını ayarlayın
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Belirli bir adla yeni bir çalışma sayfası ekleyin
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // Tüm çalışma sayfalarının adlarını çıktı olarak verin
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


