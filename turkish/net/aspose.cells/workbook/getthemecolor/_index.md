---
title: "Workbook.GetThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Tema rengini alır"
type: docs
url: /tr/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

Tema rengini alır.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ThemeColorType | Tema renk türü. |

### Dönüş Değeri

Tema rengi.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Accent6 için tema rengini al
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


