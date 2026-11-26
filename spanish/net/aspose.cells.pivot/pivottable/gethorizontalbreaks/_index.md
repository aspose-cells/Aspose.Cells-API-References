---
title: "PivotTable.GetHorizontalBreaks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Obtiene la lista de índices de filas de la tabla dinámica de saltos de página horizontales"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/gethorizontalbreaks/
---
## PivotTable.GetHorizontalBreaks method

Obtiene la lista de índices de filas de la tabla dinámica de saltos de página horizontales

```csharp
[Obsolete("Use ivotTable.GetHorizontalPageBreaks() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetHorizontalBreaks()
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.GetHorizontalPageBreaks(). Este método será eliminado 12 meses después desde diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodGetHorizontalBreaksDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcular datos para rellenar la tabla dinámica
            pivotTable.CalculateData();

            try
            {
                // Obtener saltos horizontales (saltos de página) para la tabla dinámica
                ArrayList horizontalBreaks = pivotTable.GetHorizontalBreaks();
                
                Console.WriteLine("Horizontal breaks (row indices):");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }

                // Agregar un salto de página en la fila 3 para demostración
                worksheet.HorizontalPageBreaks.Add("A3");
                
                // Obtener los saltos horizontales actualizados
                horizontalBreaks = pivotTable.GetHorizontalBreaks();
                Console.WriteLine("\nHorizontal breaks after adding page break:");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetHorizontalBreaks method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("PivotTableGetHorizontalBreaksDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


