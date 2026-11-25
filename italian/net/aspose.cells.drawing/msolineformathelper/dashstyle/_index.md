---
title: "MsoLineFormatHelper.DashStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormatHelper. Ottiene o imposta lo stile tratteggiato per la linea specificata"
type: docs
url: /it/net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Ottiene o imposta lo stile di tratteggio per la linea specificata.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // Visualizza il valore corrente di DashStyle
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // Imposta un nuovo valore di DashStyle (poiché è leggibile/scrivibile)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // Salva il risultato
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


