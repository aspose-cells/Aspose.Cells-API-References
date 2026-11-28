---
title: "WorkbookSettings.RemovePersonalInformation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Belirtilen çalışma kitabından kişisel bilgilerin kaldırılabilmesi durumunda True."
type: docs
url: /tr/net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

Belirtilen çalışma kitabından kişisel bilgiler kaldırılabiliyorsa doğru döner.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // RemovePersonalInformation özelliğini true olarak ayarlayın
            workbook.Settings.RemovePersonalInformation = true;
            
            // Örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Email");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue("john@example.com");
            
            // Çalışma kitabını kaydedin
            string outputPath = "output_with_personal_info_removed.xlsx";
            workbook.Save(outputPath);
            
            // Ayarı doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("RemovePersonalInformation setting: " + 
                loadedWorkbook.Settings.RemovePersonalInformation);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


