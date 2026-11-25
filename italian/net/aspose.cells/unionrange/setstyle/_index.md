---
title: "UnionRange.SetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnionRange. Imposta lo stile dell'intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/setstyle/
---
## UnionRange.SetStyle method

Imposta lo stile dell'intervallo.

```csharp
public void SetStyle(Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | L'oggetto Style. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio nell'intervallo A1:B2
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue("Total");
            worksheet.Cells["B2"].PutValue(456);

            // Crea un UnionRange che copre le celle A1:B2
            UnionRange unionRange = worksheet.Cells
                .CreateRange("A1:B2")
                .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Crea un'istanza di Style e imposta alcune formattazioni
                Style style = new Style();
                style.BackgroundColor = Color.LightYellow;
                style.ForegroundColor = Color.DarkBlue;
                style.HorizontalAlignment = TextAlignmentType.Center;
                style.VerticalAlignment = TextAlignmentType.Center;
                style.IsTextWrapped = true;

                // Applica lo stile all'UnionRange
                unionRange.SetStyle(style);

                Console.WriteLine("SetStyle executed successfully on the UnionRange.");

                // Salva la cartella di lavoro per visualizzare il risultato
                workbook.Save("UnionRangeSetStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetStyle: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


