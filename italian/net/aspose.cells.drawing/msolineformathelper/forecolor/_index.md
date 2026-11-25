---
title: "MsoLineFormatHelper.ForeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormatHelper. Ottiene e imposta il colore di primo piano della linea del bordo"
type: docs
url: /it/net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Ottiene e imposta il colore di primo piano della linea del bordo.

```csharp
public Color ForeColor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea una forma per dimostrare la formattazione della linea
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Ottieni il formato della linea
                MsoLineFormat lineFormat = shape.LineFormat;

                // Visualizza il valore corrente di ForeColor
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // Imposta un nuovo ForeColor (poiché è leggibile/scrivibile)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // Salva il risultato
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
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

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


