---
title: "FillFormat.GradientVariant"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Restituisce la variante di gradiente per il riempimento specificato. Valido solo per Excel 2007"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/gradientvariant/
---
## FillFormat.GradientVariant property

Restituisce la variante del gradiente per il riempimento specificato. Valido solo per Excel 2007.

```csharp
public int GradientVariant { get; }
```

### Osservazioni

Può essere solo un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient nella finestra di dialogo Fill Effects. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 150);
            FillFormat fillFormat = rectangle.Fill;
            
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 2);
            Console.WriteLine("GradientVariant after SetTwoColorGradient: " + fillFormat.GradientVariant);
            
            fillFormat.SetPresetColorGradient(GradientPresetType.Gold, GradientStyleType.FromCorner, 4);
            Console.WriteLine("GradientVariant after SetPresetColorGradient: " + fillFormat.GradientVariant);
        }
    }
}
```

### Vedi anche

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


