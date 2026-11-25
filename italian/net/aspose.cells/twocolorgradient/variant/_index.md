---
title: "TwoColorGradient.Variant"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TwoColorGradient. Ottiene e imposta la variante del gradiente"
type: docs
url: /it/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

Ottiene e imposta la variante della sfumatura.

```csharp
public int Variant { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un gradiente a due colori con variante iniziale
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // Crea e applica lo stile alla cella A1
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // Visualizza il valore corrente della variante
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // Modifica il valore della variante
            gradient.Variant = 2;

            // Crea e applica lo stile modificato alla cella B1
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // Rendi le celle più alte per visualizzare i gradienti
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


