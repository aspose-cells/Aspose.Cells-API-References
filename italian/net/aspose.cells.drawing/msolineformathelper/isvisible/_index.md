---
title: "MsoLineFormatHelper.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormatHelper. Indica se l'oggetto è visibile"
type: docs
url: /it/net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Indica se l'oggetto è visibile.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
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

                // Visualizza il valore corrente di IsVisible
                Console.WriteLine("Current IsVisible: " + lineFormat.IsVisible);

                // Imposta un nuovo valore di IsVisible (poiché è leggibile/scrivibile)
                lineFormat.IsVisible = false;
                Console.WriteLine("Updated IsVisible: " + lineFormat.IsVisible);

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("Line visibility has been updated to: " + lineFormat.IsVisible);

                // Salva il risultato
                workbook.Save("IsVisibleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line visibility.");
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


