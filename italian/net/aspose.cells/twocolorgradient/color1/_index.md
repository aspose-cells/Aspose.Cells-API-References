---
title: "TwoColorGradient.Color1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TwoColorGradient. Ottiene e imposta il primo colore del gradiente"
type: docs
url: /it/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

Ottiene e imposta il primo colore della sfumatura.

```csharp
public Color Color1 { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Crea uno stile con riempimento a gradiente
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // Inizializza un gradiente a due colori
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // Applica il gradiente allo stile della cella
            cell.SetStyle(style);
            
            // Leggi il colore iniziale
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // Modifica il colore del gradiente e riapplicalo
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // Verifica l'aggiornamento
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // Dimostrazione visiva nel file di output
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


