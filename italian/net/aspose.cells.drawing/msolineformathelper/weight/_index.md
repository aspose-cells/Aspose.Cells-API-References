---
title: "MsoLineFormatHelper.Weight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormatHelper. Restituisce o imposta lo spessore della linea in unità di pt"
type: docs
url: /it/net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Restituisce o imposta lo spessore della linea, in unità di pt.

```csharp
public double Weight { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyWeightDemo
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

                // Visualizza il valore corrente di Weight
                Console.WriteLine("Current Line Weight: " + lineFormat.Weight);

                // Imposta un nuovo valore di Weight (poiché è leggibile/scrivibile)
                lineFormat.Weight = 2.5;
                Console.WriteLine("Updated Line Weight: " + lineFormat.Weight);

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("Line weight has been updated to: " + lineFormat.Weight);

                // Salva il risultato
                workbook.Save("WeightDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line weight.");
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


