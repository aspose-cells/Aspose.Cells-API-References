---
title: "ValidationCollection.RemoveArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ValidationCollection. Rimuove tutte le impostazioni di convalida sull'intervallo"
type: docs
url: /it/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

Rimuove tutte le impostazioni di convalida sull'intervallo..

```csharp
public void RemoveArea(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'intervallo che contiene le impostazioni di convalida. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una convalida in un'area specifica
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // Creare un'area da rimuovere dalla convalida
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // Chiamare il metodo RemoveArea con il parametro CellArea
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // Visualizzare le aree di convalida rimanenti
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


