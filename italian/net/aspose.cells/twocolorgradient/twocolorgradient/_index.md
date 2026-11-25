---
title: "TwoColorGradient.TwoColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore TwoColorGradient."
type: docs
url: /it/net/aspose.cells/twocolorgradient/twocolorgradient/
---
## TwoColorGradient constructor

```csharp
public TwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | Color |  |
| color2 | Color |  |
| gradientStyleType | GradientStyleType |  |
| variant | Int32 |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class TwoColorGradientMethodSharpctorWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di TwoColorGradient utilizzando il costruttore con tutti i parametri
                TwoColorGradient gradient = new TwoColorGradient(
                    Color.LightBlue,
                    Color.DarkBlue,
                    GradientStyleType.Horizontal,
                    1);

                // Visualizza le proprietà del gradiente per verificare l'inizializzazione
                Console.WriteLine($"Gradient created with:");
                Console.WriteLine($"Color1: {gradient.Color1}");
                Console.WriteLine($"Color2: {gradient.Color2}");
                Console.WriteLine($"GradientStyleType: {gradient.GradientStyleType}");
                Console.WriteLine($"Variant: {gradient.Variant}");

                // Crea una cartella di lavoro e applica il gradiente per dimostrare la funzionalità
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Applica il gradiente a una cella
                Style style = workbook.CreateStyle();
                style.SetTwoColorGradient(
                    gradient.Color1,
                    gradient.Color2,
                    gradient.GradientStyleType,
                    gradient.Variant);

                worksheet.Cells["A1"].PutValue("TwoColorGradient Demo");
                worksheet.Cells["A1"].SetStyle(style);

                // Salva la cartella di lavoro
                workbook.Save("TwoColorGradientDemo.xlsx");
                Console.WriteLine("Gradient applied successfully to workbook.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


