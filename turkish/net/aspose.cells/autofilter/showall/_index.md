---
title: "AutoFilter.ShowAll"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Tüm satırların gizliliğini kaldır"
type: docs
url: /tr/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Tüm satırların gizlemesini kaldır.

```csharp
public void ShowAll()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Sadece "Apple" gösterecek şekilde filtrele
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // Tüm verileri tekrar göster
            worksheet.AutoFilter.ShowAll();
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


