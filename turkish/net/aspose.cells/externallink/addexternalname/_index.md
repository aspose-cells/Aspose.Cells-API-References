---
title: "ExternalLink.AddExternalName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLink yöntemi. Dış bir ad ekler"
type: docs
url: /tr/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Harici bir ad ekler.

```csharp
public void AddExternalName(string text, string referTo)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | Dış adın metni. Dış ad bir çalışma sayfasına aitse, metin Sheet1!Text şeklinde olmalıdır. |
| referTo | String | Dış adın referTo değeri. Bir hücre ya da aralık olmalıdır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek bir dış çalışma kitabı oluşturun
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // Ana çalışma kitabına dış bağlantı ekleyin
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // Dış ad ekle
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // Formülde dış adı kullanın
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // Formülü hesapla
            workbook.CalculateFormula();
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


