---
title: "Enum ErrorCellValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ErrorCellValueType enum. Rappresenta un valore di cella che contiene un errore"
type: docs
url: /it/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Rappresenta un valore di cella che contiene un errore.

```csharp
public enum ErrorCellValueType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Value | `1` | Rappresenta il valore di una cella contenente un errore #VALUE!. |
| Ref | `3` | Rappresenta il valore di una cella contenente un errore #REF!. |
| Name | `4` | Rappresenta il valore di una cella contenente un errore #NAME?. |
| NA | `6` | Rappresenta il valore di una cella contenente un errore #N/A. |
| Blocked | `10` | Rappresenta il valore di una cella contenente un errore #BLOCKED!. |
| Busy | `14` | Rappresenta il valore di una cella contenente un errore #BUSY!. |
| Calc | `13` | Rappresenta il valore di una cella contenente un errore #CALC!. |
| Connect | `9` | Rappresenta il valore di una cella contenente un errore #CONNECT!. |
| Field | `12` | Rappresenta il valore di una cella contenente un errore #FIELD!. |
| Spill | `8` | Rappresenta il valore di una cella contenente un errore #SPILL!. |
| Unknown | `11` | Rappresenta il valore di una cella contenente un errore #UNKNOWN!. |
| TimeOut | `19` | Rappresenta il valore di una cella contenente un errore #TIMEOUT!. |
| External | `18` | Rappresenta il valore di una cella contenente un errore #EXTERNAL!. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta una formula che causerà un errore spill.
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // Calcola le formule per attivare l'errore.
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Errore spill previsto.
            }
            
            // Ottieni il valore ricco della cella.
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Verifica il tipo di errore.
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


