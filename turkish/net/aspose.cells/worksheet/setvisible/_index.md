---
title: "Worksheet.SetVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Görünür seçenekleri ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Görünür seçenekleri ayarlar.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isVisible | Boolean | Çalışma sayfasının görünür olup olmadığı |
| ignoreError | Boolean | Bu seçenek geçerli değilse hatayı yok sayıp yok saymayacağını belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Çalışma sayfalarının görünürlüğünü ayarla
            // İlk parametre: isVisible - sayfayı gizlemek için false
            // İkinci parametre: ignoreError - sayfa gizlenemiyorsa hatayı yok saymak için true
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


