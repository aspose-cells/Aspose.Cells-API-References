---
title: "Validation.RemoveArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di convalida. Rimuove le impostazioni di convalida nell'intervallo"
type: docs
url: /it/net/aspose.cells/validation/removearea/
---
## Validation.RemoveArea method

Rimuovi le impostazioni di convalida nell'intervallo.

```csharp
public void RemoveArea(CellArea cellArea)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | CellArea | le aree in cui queste impostazioni di convalida dovrebbero essere rimosse. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una convalida al foglio di lavoro
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Aggiungi l'area di convalida iniziale
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            validation.AddArea(initialArea);

            // Aggiungi un'altra area alla convalida
            CellArea additionalArea = CellArea.CreateCellArea(1, 1, 1, 1);
            validation.AddArea(additionalArea);

            Console.WriteLine("Validation areas count after adding: " + validation.Areas.Length);

            // Rimuovi l'area aggiuntiva
            validation.RemoveArea(additionalArea);

            Console.WriteLine("Validation areas count after removing: " + validation.Areas.Length);

            // Aggiungi più aree
            CellArea[] multipleAreas = new CellArea[]
            {
                CellArea.CreateCellArea(2, 2, 2, 2),
                CellArea.CreateCellArea(3, 3, 3, 3),
                CellArea.CreateCellArea(4, 4, 4, 4)
            };
            validation.AddAreas(multipleAreas, false, false);

            Console.WriteLine("Validation areas count after adding multiple: " + validation.Areas.Length);

            // Rimuovi una delle aree
            validation.RemoveArea(multipleAreas[1]);

            Console.WriteLine("Validation areas count after removing one: " + validation.Areas.Length);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


