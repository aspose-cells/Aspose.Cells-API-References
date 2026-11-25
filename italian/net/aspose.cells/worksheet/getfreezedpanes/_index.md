---
title: "Worksheet.GetFreezedPanes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Ottiene i riquadri congelati"
type: docs
url: /it/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

Ottiene i riquadri congelati.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32& | Indice della riga. |
| colonna | Int32& | Indice colonna. |
| freezedRows | Int32& | Numero di righe visibili nel riquadro superiore, non più dell'indice di riga. |
| freezedColumns | Int32& | Numero di colonne visibili nel riquadro sinistro, non più dell'indice di colonna. |

### Valore di ritorno

Restituisce se il foglio di lavoro è congelato

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Congela i riquadri nella cella C5 (riga 4, colonna 2) con 2 righe congelate e 1 colonna congelata
            worksheet.FreezePanes(4, 2, 2, 1);

            // Dichiarare le variabili per memorizzare le informazioni dei riquadri congelati
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // Chiamare il metodo GetFreezedPanes con parametri out
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // Visualizza i risultati
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // Salva la cartella di lavoro
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


