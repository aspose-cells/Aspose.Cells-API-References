---
title: "MsoLineFormatHelper.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormatHelper. Restituisce un oggetto Style che rappresenta lo stile dell'intervallo specificato"
type: docs
url: /it/net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Restituisce un oggetto Style che rappresenta lo stile dell'intervallo specificato.

```csharp
public MsoLineStyle Style { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
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

                // Ottieni il formato della linea direttamente (MsoLineFormatHelper sembra essere una classe di supporto)
                // Poiché non possiamo istanziare MsoLineFormatHelper direttamente, lavoreremo con la proprietà LineFormat
                MsoLineFormat lineFormat = shape.LineFormat;

                // Visualizza il valore corrente di Style
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // Imposta un nuovo stile (poiché Style è leggibile/scrivibile)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // Salva il risultato
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


