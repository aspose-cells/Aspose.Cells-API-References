---
title: "TwoColorGradient.Color2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TwoColorGradient. Ottiene e imposta il secondo colore del gradiente"
type: docs
url: /it/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

Ottiene e imposta il secondo colore della sfumatura.

```csharp
public Color Color2 { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di gradiente a due colori
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // Crea il primo stile con il gradiente iniziale
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // Visualizza il valore corrente di Color2
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // Modifica la proprietà Color2
            gradient.Color2 = Color.Red;

            // Crea il secondo stile con il gradiente modificato
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // Regola le righe per la visibilità
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // Salva la cartella di lavoro
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


