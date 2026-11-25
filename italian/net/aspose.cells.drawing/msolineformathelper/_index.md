---
title: "Class MsoLineFormatHelper"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.MsoLineFormatHelper class. Rappresenta la formattazione di linee e punte di freccia"
type: docs
url: /it/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Rappresenta la formattazione di linee e punte di freccia.

```csharp
public class MsoLineFormatHelper
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Ottiene e imposta il colore di sfondo della linea del bordo. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Ottiene o imposta lo stile di tratteggio per la linea specificata. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Ottiene e imposta il colore di primo piano della linea del bordo. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Indica se l'oggetto è visibile. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Restituisce un oggetto Style che rappresenta lo stile dell'intervallo specificato. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Restituisce o imposta lo spessore della linea, in unità di pt. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una forma per dimostrare la formattazione della linea
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Ottieni il formato della linea direttamente dalla forma
                MsoLineFormat lineFormat = shape.LineFormat;

                // Imposta le proprietà direttamente sul formato della linea
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Visualizza le proprietà configurate
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Salva la cartella di lavoro
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


