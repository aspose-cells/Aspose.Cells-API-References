---
title: "PivotFilterCollection.AddValueFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilterCollection. Filtra por valores del campo de datos pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotfiltercollection/addvaluefilter/
---
## PivotFilterCollection.AddValueFilter method

Filtra por los valores del campo pivot de datos.

```csharp
public PivotFilter AddValueFilter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    double value1, double value2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | Int32 | El índice del campo en la fuente. |
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

    public class PivotFilterCollectionMethodAddValueFilterWithInt32Int32PivotFilterTypeDoublDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Widget";
            worksheet.Cells["A3"].Value = "Gadget";
            worksheet.Cells["A4"].Value = "Thingy";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 15.99;
            worksheet.Cells["B3"].Value = 24.99;
            worksheet.Cells["B4"].Value = 9.99;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Agregar filtro de valor para mostrar productos con precios entre $10 y $20
                PivotFilter filter = filters.AddValueFilter(
                    baseFieldIndex: 0,
                    valueFieldIndex: 1,
                    type: PivotFilterType.ValueBetween,
                    value1: 10.0,
                    value2: 20.0
                );

                Console.WriteLine($"Value filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding value filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddValueFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


