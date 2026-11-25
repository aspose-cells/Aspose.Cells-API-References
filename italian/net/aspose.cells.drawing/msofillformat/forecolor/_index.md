---
title: "MsoFillFormat.ForeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormat. Ottiene e imposta il colore di primo piano del riempimento"
type: docs
url: /it/net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Ottiene e imposta il colore di primo piano del riempimento.

```csharp
public Color ForeColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Ottieni il formato di riempimento
            MsoFillFormat fillFormat = rectangle.FillFormat;

            // Imposta e dimostra la proprietà ForeColor
            fillFormat.ForeColor = System.Drawing.Color.Red;
            Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);

            // Modifica il ForeColor
            fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
            Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);

            // Salva la cartella di lavoro
            workbook.Save("MsoFillFormatForeColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


