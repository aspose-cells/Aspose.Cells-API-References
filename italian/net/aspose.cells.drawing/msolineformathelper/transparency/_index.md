---
title: "MsoLineFormatHelper.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormatHelper. Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 opaco a 1.0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/msolineformathelper/transparency/
---
## MsoLineFormatHelper.Transparency property

Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyTransparencyDemo
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

                // Visualizza il valore corrente di Transparency
                Console.WriteLine("Current Transparency: " + lineFormat.Transparency);

                // Imposta un nuovo valore di Transparency (poiché è leggibile/scrivibile)
                lineFormat.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + lineFormat.Transparency);

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("Line transparency has been updated to: " + lineFormat.Transparency);

                // Salva il risultato
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line transparency.");
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


