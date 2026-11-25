---
title: "Style.GetTwoColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Ottieni l'impostazione del gradiente a due colori"
type: docs
url: /it/net/aspose.cells/style/gettwocolorgradient/
---
## Style.GetTwoColorGradient method

Ottieni l'impostazione del gradiente a due colori.

```csharp
[Obsolete("Use Style.GetTwoColorGradientSetting() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GetTwoColorGradient(out Color color1, out Color color2, 
    out GradientStyleType gradientStyleType, out int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | Color& | Un colore di gradiente. |
| color2 | Color& | Due colori di gradiente. |
| gradientStyleType | GradientStyleType& | Stile di sfumatura del gradiente. |
| variant | Int32& | La variante del gradiente. |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Style.GetTwoColorGradientSetting(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientWithColorColorGradientStyleTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile e imposta un gradiente a due colori
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Two Color Gradient Demo");

            // Prepara le variabili per ottenere le impostazioni del gradiente
            Color color1 = Color.Empty;
            Color color2 = Color.Empty;
            GradientStyleType gradientStyle = GradientStyleType.Horizontal;
            int variant = 0;

            try
            {
                // Chiama il metodo GetTwoColorGradient
#pragma warning disable CS0618 // Type or member is obsolete
                style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
#pragma warning restore CS0618 // Type or member is obsolete

                // Visualizza le impostazioni del gradiente recuperate
                Console.WriteLine("Gradient Settings:");
                Console.WriteLine($"Color1: {color1}");
                Console.WriteLine($"Color2: {color2}");
                Console.WriteLine($"Gradient Style: {gradientStyle}");
                Console.WriteLine($"Variant: {variant}");

                // Salva la cartella di lavoro
                workbook.Save("StyleMethodGetTwoColorGradientDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradient method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


