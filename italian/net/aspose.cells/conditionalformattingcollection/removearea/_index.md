---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ConditionalFormattingCollection. Rimuovi tutta la formattazione condizionale nell'intervallo"
type: docs
url: /it/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

Rimuove tutta la formattazione condizionale nell'intervallo.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La riga iniziale dell'intervallo. |
| startColumn | Int32 | La colonna iniziale dell'intervallo. |
| totalRows | Int32 | Il numero di righe dell'intervallo. |
| totalColumns | Int32 | Il numero di colonne dell'intervallo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la raccolta di formattazione condizionale
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // Aggiungi alcune regole di formattazione condizionale
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // Chiama RemoveArea con i parametri (Int32, Int32, Int32, Int32)
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // Verifica l'effetto controllando il conteggio (sarebbe 0 se tutta la formattazione è stata rimossa)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


