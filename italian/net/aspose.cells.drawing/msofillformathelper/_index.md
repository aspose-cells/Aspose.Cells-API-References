---
title: "Class MsoFillFormatHelper"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.MsoFillFormatHelper class. Rappresenta la formattazione di riempimento per una forma"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/
---
## MsoFillFormatHelper class

Rappresenta la formattazione di riempimento per una forma.

```csharp
public class MsoFillFormatHelper
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformathelper/backcolor/) { get; set; } | Ottiene e imposta il colore di sfondo del file. |
| [ForeColor](../../aspose.cells.drawing/msofillformathelper/forecolor/) { get; set; } | Ottiene e imposta il colore di primo piano del riempimento. |
| [ForeColorTransparency](../../aspose.cells.drawing/msofillformathelper/forecolortransparency/) { get; set; } | Restituisce o imposta il grado del colore di primo piano del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [ImageData](../../aspose.cells.drawing/msofillformathelper/imagedata/) { get; set; } | Ottiene e imposta i dati di riempimento Texture e Picture. |
| [IsVisible](../../aspose.cells.drawing/msofillformathelper/isvisible/) { get; set; } | Indica se è presente un riempimento. |
| [Texture](../../aspose.cells.drawing/msofillformathelper/texture/) { get; } | Ottiene il tipo di riempimento texture. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformathelper/setonecolorgradient/)(Color, double, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a un colore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class DrawingClassMsoFillFormatHelperDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "MsoFillFormatHelper Demo";

            try
            {
                // Crea un'istanza di MsoFillFormatHelper usando la riflessione
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Imposta le proprietà di base
                fillHelper.ForeColor = Color.FromArgb(255, 100, 150, 200);
                fillHelper.ForeColorTransparency = 0.3;
                fillHelper.BackColor = Color.LightGray;
                fillHelper.IsVisible = true;

                // Visualizza i valori delle proprietà
                Console.WriteLine($"ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency: {fillHelper.ForeColorTransparency}");
                Console.WriteLine($"BackColor: {fillHelper.BackColor}");
                Console.WriteLine($"IsVisible: {fillHelper.IsVisible}");
                Console.WriteLine($"Texture (read-only): {fillHelper.Texture}");

                // Salva la cartella di lavoro
                workbook.Save("MsoFillFormatHelperDemo.xlsx");
                Console.WriteLine("MsoFillFormatHelper demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MsoFillFormatHelper demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


