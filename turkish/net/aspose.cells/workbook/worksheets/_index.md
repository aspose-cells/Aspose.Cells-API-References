---
title: "Workbook.Worksheets"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Elektronik tabloda WorksheetCollection koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Elektronik tabloda [`WorksheetCollection`](../../worksheetcollection/) koleksiyonunu alır.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Dönüş Değeri

[`WorksheetCollection`](../../worksheetcollection/) collection

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Yeni bir çalışma sayfası ekle
            workbook.Worksheets.Add("SecondSheet");
            
            // İkinci çalışma sayfasına eriş ve veri ekle
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // Çalışma sayfası sayısını çıktıla
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


