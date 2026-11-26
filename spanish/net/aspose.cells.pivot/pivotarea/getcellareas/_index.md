---
title: "PivotArea.GetCellAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotArea. Obtiene las áreas de celdas de esta área de pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/getcellareas/
---
## PivotArea.GetCellAreas method

Obtiene las áreas de celdas de esta área de tabla dinámica.

```csharp
public CellArea[] GetCellAreas()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaMethodGetCellAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos mínimos de tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";

            try
            {
                // Crear tabla dinámica con configuración básica
                int pivotIndex = worksheet.PivotTables.Add("A1:A3", "D1", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Inicializar el área de pivote con la instancia de la tabla dinámica
                PivotArea pivotArea = new PivotArea(pivotTable);

                // Configurar ajustes del área de pivote
                pivotArea.RuleType = PivotAreaType.Normal;
                pivotArea.AxisType = PivotFieldType.Data;
                pivotArea.IsRowGrandIncluded = true;

                // Ejecutar método objetivo
                CellArea[] cellAreas = pivotArea.GetCellAreas();

                Console.WriteLine($"GetCellAreas returned {cellAreas.Length} cell area(s)");
                foreach (CellArea area in cellAreas)
                {
                    Console.WriteLine($"CellArea: Columns {area.StartColumn}-{area.EndColumn}, Rows {area.StartRow}-{area.EndRow}");
                }

                workbook.Save("GetCellAreasDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetCellAreas: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


