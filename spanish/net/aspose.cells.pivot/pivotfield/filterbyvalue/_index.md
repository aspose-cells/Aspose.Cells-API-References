---
title: "PivotField.FilterByValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Filtra por valores del campo dinámico de datos"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/filterbyvalue/
---
## PivotField.FilterByValue method

Filtra por los valores del campo pivot de datos.

```csharp
public PivotFilter FilterByValue(int valueFieldIndex, PivotFilterType type, double value1, 
    double value2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valueFieldIndex | Int32 | El índice del campo de valor en la región de valores. |
| type | PivotFilterType | El tipo de datos de filtrado. |
| value1 | Double | El valor de la condición de filtro |
| value2 | Double | El valor límite superior de la condición de filtro entre |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodFilterByValueWithInt32PivotFilterTypeDoubleDoubDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["B3"].Value = 1.8;
            worksheet.Cells["B4"].Value = 3.2;
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["C2"].Value = 100;
            worksheet.Cells["C3"].Value = 150;
            worksheet.Cells["C4"].Value = 80;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campos de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Llamar al método FilterByValue con los parámetros (Int32, PivotFilterType, Double, Double)
                // Filtrar productos donde Cantidad (índice de campo 1) está entre 90 y 160
                PivotFilter filter = pivotField.FilterByValue(1, PivotFilterType.ValueBetween, 90.0, 160.0);

                Console.WriteLine("FilterByValue method executed successfully");
                Console.WriteLine($"Filter type: {filter.FilterType}");
                Console.WriteLine($"Value field index: {filter.ValueFieldIndex}");

                // Actualiza la tabla dinámica para mostrar los cambios
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FilterByValue method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotFieldMethodFilterByValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


