---
title: "Cells.GetFirstDataRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'indice della prima riga della cella che contiene dati nella colonna specificata"
type: docs
url: /it/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Restituisce l'indice della prima riga della cella che contiene dati nella colonna specificata.

```csharp
public int GetFirstDataRow(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |

### Valore di ritorno

indice della prima riga.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per dimostrare il metodo
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Ottieni la raccolta Cells dal foglio di lavoro
                Cells cells = worksheet.Cells;

                // Chiama GetFirstDataRow per la colonna A (indice 0)
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Chiama GetFirstDataRow per la colonna B (indice 1)
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Chiama GetFirstDataRow per la colonna C (indice 2)
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Salva la cartella di lavoro
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


