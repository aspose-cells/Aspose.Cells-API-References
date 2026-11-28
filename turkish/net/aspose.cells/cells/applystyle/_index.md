---
title: "Cells.ApplyStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Tüm çalışma sayfasına biçimler uygular"
type: docs
url: /tr/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Tüm bir çalışma sayfası için biçimleri uygular.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Uygulanacak stil nesnesi. |
| bayrak | StyleFlag | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = wb.Worksheets[0];
            
            // Bir stil oluşturun ve metin kaydırmayı ayarlayın
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // Stil bayrağı oluşturun ve metin kaydırma bayrağını etkinleştirin
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Stili çalışma sayfasındaki tüm hücrelere uygulayın
            sheet.Cells.ApplyStyle(style, flag);
            
            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


