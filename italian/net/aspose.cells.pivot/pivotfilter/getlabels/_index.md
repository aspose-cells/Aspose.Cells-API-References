---
title: "PivotFilter.GetLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilter. Ottiene le etichette del filtro di didascalia"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/getlabels/
---
## PivotFilter.GetLabels method

Restituisce le etichette del filtro didascalia.

```csharp
public string[] GetLabels()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterMethodGetLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una struttura di tabella pivot valida
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                
                // Crea una tabella pivot con i parametri corretti
                int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Crea un filtro pivot con parametri validi
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Configura le proprietà del filtro
                pivotFilter.Name = "SampleFilter";
                pivotFilter.EvaluationOrder = 1;

                // Esegui il metodo GetLabels
                string[] labels = pivotFilter.GetLabels();

                Console.WriteLine($"Retrieved {labels?.Length ?? 0} labels:");
                if (labels != null)
                {
                    foreach (string label in labels)
                    {
                        Console.WriteLine($"- {label}");
                    }
                }

                workbook.Save("GetLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLabels: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


