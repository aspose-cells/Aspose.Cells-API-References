---
title: "PivotFilter.GetLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilter. Obtiene las etiquetas del filtro de título"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/getlabels/
---
## PivotFilter.GetLabels method

Obtiene las etiquetas del filtro de título.

```csharp
public string[] GetLabels()
```

### Ejemplos

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
                // Cree una estructura de tabla dinámica válida
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                
                // Crea una tabla dinámica con los parámetros correctos
                int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Cree un filtro pivote con parámetros válidos
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Configure las propiedades del filtro
                pivotFilter.Name = "SampleFilter";
                pivotFilter.EvaluationOrder = 1;

                // Ejecute el método GetLabels
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

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


