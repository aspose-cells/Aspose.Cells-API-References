---
title: "WorksheetCollection.ActiveSheetName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Elektronik tablo açıldığında aktif çalışma sayfasının adını temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Elektronik tablo açıldığında etkin çalışma sayfasının adını temsil eder.

```csharp
public string ActiveSheetName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Aktif sayfayı adla ayarlayın
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // Etkin sayfayı doğrula
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


