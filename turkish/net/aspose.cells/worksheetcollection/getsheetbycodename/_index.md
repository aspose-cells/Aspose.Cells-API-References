---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Çalışma sayfasını kod adına göre alır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Kod adıyla çalışma sayfasını alır.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| codeName | String | Çalışma sayfası kod adı. |

### Dönüş Değeri

Belirtilen kod adına sahip öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfalarını ekle ve kod adlarını ayarla
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // Kod adına göre çalışma sayfasını al
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // Hücrelere yazarak kullanımını göster
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // Çalışma kitabını kaydedin
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


