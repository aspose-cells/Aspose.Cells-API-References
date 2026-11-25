---
title: "ThemeColor.ColorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThemeColor. Ottiene e imposta il tipo di tema"
type: docs
url: /it/net/aspose.cells/themecolor/colortype/
---
## ThemeColor.ColorType property

Ottiene e imposta il tipo di tema.

```csharp
public ThemeColorType ColorType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyColorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea due colori del tema con tipi diversi
            ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
            ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
            
            // Dimostra la proprietà ColorType
            Console.WriteLine("Color1 Type: " + color1.ColorType);
            Console.WriteLine("Color2 Type: " + color2.ColorType);
            
            // Applica i colori del tema alle celle
            Style style1 = workbook.CreateStyle();
            style1.ForegroundThemeColor = color1;
            worksheet.Cells["A1"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundThemeColor = color2;
            worksheet.Cells["A2"].SetStyle(style2);
            
            // Salva la cartella di lavoro
            workbook.Save("ThemeColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


