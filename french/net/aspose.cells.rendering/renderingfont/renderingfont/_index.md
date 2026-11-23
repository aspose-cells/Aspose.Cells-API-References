---
title: "RenderingFont.RenderingFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur RenderingFont. Initialise une nouvelle instance de RenderingFont"
type: docs
url: /fr/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Initialise une nouvelle instance de [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontName | String | nom de police |
| fontSize | Single | taille de police en points |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontMethodCtorWithStringSingleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez une police en utilisant le constructeur #ctor(string, single)
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // Créez le style et définissez la police
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // Appliquez le style à la cellule
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


