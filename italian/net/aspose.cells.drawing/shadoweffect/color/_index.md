---
title: "ShadowEffect.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShadowEffect. Ottiene e imposta il colore dell'ombra"
type: docs
url: /it/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Ottiene e imposta il colore dell'ombra.

```csharp
public CellsColor Color { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare l'effetto ombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Ottieni l'effetto ombra dalla forma
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Crea un nuovo oggetto CellsColor
                CellsColor shadowColor = workbook.CreateCellsColor();

                // Imposta il colore su rosso usando i valori RGB
                shadowColor.Color = Color.Red;

                // Applica il colore all'effetto ombra
                shadowEffect.Color = shadowColor;

                // Visualizza il valore corrente del colore
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Salva la cartella di lavoro per dimostrare l'effetto
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Carica nuovamente la cartella di lavoro per verificare che il colore sia stato salvato
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Visualizza il valore del colore caricato
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


