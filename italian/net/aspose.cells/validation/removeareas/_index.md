---
title: "Validation.RemoveAreas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di convalida. Rimuove questa convalida dalle aree specificate"
type: docs
url: /it/net/aspose.cells/validation/removeareas/
---
## Validation.RemoveAreas method

Rimuove questa convalida dalle aree specificate.

```csharp
public void RemoveAreas(CellArea[] areas)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| aree | CellArea[] | le aree in cui queste impostazioni di convalida dovrebbero essere rimosse. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi la convalida dei dati al foglio di lavoro
            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            
            // Configura le impostazioni di convalida
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "10";

            // Crea due aree di celle per la convalida
            CellArea area1 = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 1,
                EndColumn = 1
            };  // A1:B2
            CellArea area2 = new CellArea
            {
                StartRow = 2,
                StartColumn = 2,
                EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
                EndColumn = 3
            };  // C3:D4 (corrected end coordinates)
            
            // Aggiungi le aree alla convalida
            validation.AddArea(area1);
            validation.AddArea(area2);
            Console.WriteLine($"Added areas: {validation.Areas.Length}");

            try
            {
                // Crea un array con un'area da rimuovere
                CellArea[] removeAreas = { area1 };
                
                // Esegui il metodo RemoveAreas
                validation.RemoveAreas(removeAreas);
                Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
                
                // Visualizza le coordinate delle aree rimanenti
                foreach (CellArea remainingArea in validation.Areas)
                {
                    Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Salvare la cartella di lavoro modificata
            workbook.Save("ValidationRemoveAreasDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


