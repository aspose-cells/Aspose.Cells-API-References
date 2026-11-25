---
title: "MsoFillFormatHelper.ForeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormatHelper. Ottiene e imposta il colore di primo piano del riempimento"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Ottiene e imposta il colore di primo piano del riempimento.

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
    using System.Reflection;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'etichetta per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "ForeColor Property Demo";

            try
            {
                // Crea un'istanza di MsoFillFormatHelper usando la riflessione (senza costruttore pubblico)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visualizza il valore predefinito di ForeColor
                Console.WriteLine($"Default ForeColor: {fillHelper.ForeColor}");

                // Imposta un nuovo valore di ForeColor
                fillHelper.ForeColor = Color.FromArgb(255, 128, 0, 128); // Purple color
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");

                // Dimostra come ottenere il valore di ForeColor
                Color currentColor = fillHelper.ForeColor;
                Console.WriteLine($"Current ForeColor (RGB): R={currentColor.R}, G={currentColor.G}, B={currentColor.B}");

                // Salva la cartella di lavoro per dimostrare l'esecuzione corretta
                workbook.Save("ForeColorDemo.xlsx");

                Console.WriteLine("ForeColor property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColor demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


