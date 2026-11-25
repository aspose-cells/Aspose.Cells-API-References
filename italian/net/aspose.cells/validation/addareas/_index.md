---
title: "Validation.AddAreas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Validation. Applica la convalida alle aree specificate"
type: docs
url: /it/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

Applica la convalida alle aree specificate.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| aree | CellArea[] | Le aree. |
| checkIntersection | Booleano | Se verificare l'intersezione dell'area fornita con le aree delle convalide esistenti. Se una convalida è stata applicata nell'area fornita (o in una sua parte), allora la convalida esistente dovrebbe essere rimossa prima dall'area fornita. Altrimenti potrebbe verificarsi corruzione per le Validations generate. Se l'utente è sicuro che tutte le aree aggiunte non si intersecano con alcuna area esistente, questo parametro può essere impostato su false per motivi di prestazioni. |
| checkEdge | Booleano | Se verificare il bordo delle aree applicate da questa Validation. Le impostazioni interne della Validation dipendono da quella in alto a sinistra dei suoi intervalli applicati, quindi se una delle aree fornite diventerà la nuova in alto a sinistra degli intervalli applicati, le impostazioni interne dovrebbero essere modificate e ricostruite, altrimenti potrebbe verificarsi un risultato inatteso. Se l'utente è sicuro che nessuna di queste aree aggiunte sia la in alto a sinistra, questo parametro può essere impostato su false per motivi di prestazioni. |

### Osservazioni

In questo metodo, rimuoveremo tutte le vecchie convalide nell'area fornita. Per l'area in alto a sinistra degli intervalli applicati di Validation, prima il suo StartRow è il più piccolo, poi il suo StartColumn è il più piccolo tra le aree che hanno lo stesso StartRow minimo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


