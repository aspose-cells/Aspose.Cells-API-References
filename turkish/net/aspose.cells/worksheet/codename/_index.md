---
title: "Worksheet.CodeName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasının kod adını alır."
type: docs
url: /tr/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Çalışma sayfası kod adını alır.

```csharp
public string CodeName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Varsayılan CodeName'i göster.
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // CodeName'i değiştir.
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // Yeni bir çalışma sayfası ekleyin ve CodeName'ini gösterin.
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


