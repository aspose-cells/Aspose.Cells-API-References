---
title: "Classe MsoFillFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.MsoFillFormat. Rappresenta la formattazione di riempimento per una forma"
type: docs
url: /it/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

Rappresenta la formattazione di riempimento per una forma.

```csharp
public class MsoFillFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Ottiene e imposta il colore di sfondo del file. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Ottiene e imposta il colore di primo piano del riempimento. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Ottiene e imposta i dati di riempimento Texture e Picture. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Indica se è presente un riempimento. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Ottiene il tipo di riempimento texture. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a un colore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma ad arco al foglio di lavoro
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Accedi al formato di riempimento della forma
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Imposta il colore di primo piano del riempimento
            fillFormat.ForeColor = Color.Blue;

            // Imposta il colore di sfondo del riempimento
            fillFormat.BackColor = Color.LightBlue;

            // Imposta la trasparenza
            fillFormat.Transparency = 0.5;

            // Verifica se il riempimento è visibile
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Imposta un riempimento a gradiente monocolore
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Salva la cartella di lavoro
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


