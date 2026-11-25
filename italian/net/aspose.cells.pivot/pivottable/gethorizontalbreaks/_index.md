---
title: "PivotTable.GetHorizontalBreaks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Ottiene l'elenco degli indici di riga della tabella pivot dei interruzioni di pagina orizzontali"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/gethorizontalbreaks/
---
## PivotTable.GetHorizontalBreaks method

Ottiene l'elenco degli indici di riga della tabella pivot delle interruzioni di pagina orizzontali

```csharp
[Obsolete("Use ivotTable.GetHorizontalPageBreaks() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetHorizontalBreaks()
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotTable.GetHorizontalPageBreaks(). Questo metodo sarà rimosso 12 mesi dopo a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodGetHorizontalBreaksDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcola i dati per popolare la tabella pivot
            pivotTable.CalculateData();

            try
            {
                // Ottieni le interruzioni orizzontali (interruzioni di pagina) per la tabella pivot
                ArrayList horizontalBreaks = pivotTable.GetHorizontalBreaks();
                
                Console.WriteLine("Horizontal breaks (row indices):");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }

                // Aggiungi un'interruzione di pagina alla riga 3 per dimostrazione
                worksheet.HorizontalPageBreaks.Add("A3");
                
                // Ottieni le interruzioni orizzontali aggiornate
                horizontalBreaks = pivotTable.GetHorizontalBreaks();
                Console.WriteLine("\nHorizontal breaks after adding page break:");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetHorizontalBreaks method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("PivotTableGetHorizontalBreaksDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


