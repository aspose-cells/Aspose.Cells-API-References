---
title: "Workbook.RemovePersonalInformation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Kişisel bilgileri kaldırır"
type: docs
url: /tr/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Kişisel bilgileri kaldırır.

```csharp
public void RemovePersonalInformation()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Yazar bilgileriyle bir yorum ekle
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // Orijinal yazar bilgisini göster
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // Kişisel bilgileri kaldır
            wb.RemovePersonalInformation();
            
            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Kaldırmayı doğrulamak için yeniden yükle
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


