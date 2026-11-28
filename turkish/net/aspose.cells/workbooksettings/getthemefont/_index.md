---
title: "WorkbookSettings.GetThemeFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings yöntemi. Varsayılan tema yazı tipi adını alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Varsayılan tema yazı tipi adını alır.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | FontSchemeType | Yazı tipinin şema türü. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Küçük şema türü için varsayılan tema yazı tipini alın
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // Büyük şema türü için varsayılan tema yazı tipini alın
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


