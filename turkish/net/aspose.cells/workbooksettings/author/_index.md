---
title: "WorkbookSettings.Author"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Dosyanın yazarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

Dosyanın yazarını alır ve ayarlar.

```csharp
public string Author { get; set; }
```

### Açıklamalar

Ayarlanmamış, önce [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/) kontrol edin, ardından Environment'ın kullanıcısını kontrol edin.

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            // Yazar özelliğini ayarla
            settings.Author = "John Doe";

            // Çalışma kitabı işlevselliğini göstermek için örnek veri ekle
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // Çalışma kitabını kaydedin
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


