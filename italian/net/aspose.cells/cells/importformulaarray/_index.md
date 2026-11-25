---
title: "Cells.ImportFormulaArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa un array di formule in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/importformulaarray/
---
## Cells.ImportFormulaArray method

Importa un array di formula in un foglio di lavoro.

```csharp
public void ImportFormulaArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringArray | String[] | Array di formule. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| isVertical | Booleano | Specifica se importare i dati verticalmente o orizzontalmente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Prepara l'array di formule e i parametri
            string[] formulas = new string[] { "=A1+B1", "=C1*D1" };
            int firstRow = 0;
            int firstColumn = 0;
            bool isVertical = true;

            try
            {
                // Importa le formule verticalmente a partire dalla cella A1
                worksheet.Cells.ImportFormulaArray(formulas, firstRow, firstColumn, isVertical);
                
                // Imposta i valori per i riferimenti di formula
                worksheet.Cells["A1"].PutValue(2);
                worksheet.Cells["B1"].PutValue(3);
                worksheet.Cells["C1"].PutValue(4);
                worksheet.Cells["D1"].PutValue(5);
                
                // Calcola le formule
                workbook.CalculateFormula();

                Console.WriteLine("Formulas imported successfully. Calculated results:");
                Console.WriteLine($"A2 value: {worksheet.Cells["A2"].Value}"); // Should be 5
                Console.WriteLine($"A3 value: {worksheet.Cells["A3"].Value}"); // Should be 20
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportFormulaArray method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


