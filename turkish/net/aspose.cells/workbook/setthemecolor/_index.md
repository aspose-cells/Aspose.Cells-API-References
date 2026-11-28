---
title: "Workbook.SetThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Tema rengini ayarlar"
type: docs
url: /tr/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Tema rengini ayarlar

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ThemeColorType | Tema renk türü. |
| color | Color | tema rengi |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Text1 için tema rengini Yeşil olarak ayarla
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // Tema rengini varsayılan stile uygula
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


