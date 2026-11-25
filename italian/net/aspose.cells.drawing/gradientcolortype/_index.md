---
title: "Enum GradientColorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.GradientColorType. Rappresenta il tipo di colore del gradiente per il riempimento specificato"
type: docs
url: /it/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Rappresenta il tipo di colore gradiente per il riempimento specificato.

```csharp
public enum GradientColorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessun colore di gradiente |
| OneColor | `1` | Un colore di gradiente |
| PresetColors | `2` | Colori di gradiente predefiniti |
| TwoColors | `3` | Due colori sfumati |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una forma per dimostrare il riempimento sfumato
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Imposta il tipo di riempimento sfumato
                fill.FillType = FillType.Gradient;

                // Dimostra i diversi valori dell'enumerazione GradientColorType
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Leggi e visualizza il tipo di colore sfumato corrente (la proprietà è sola lettura)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Salva la cartella di lavoro
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


