---
title: "PivotFilterCollection.AddTop10Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilterCollection. Filtra por valores del campo de datos pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotfiltercollection/addtop10filter/
---
## PivotFilterCollection.AddTop10Filter method

Filtra por los valores del campo pivot de datos.

```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    bool isTop, int itemCount)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | Int32 | El índice del campo en la fuente. |
| valueFieldIndex | Int32 | El índice del campo de datos en la región de datos. |
| type | PivotFilterType | El tipo de filtrado de datos. Sólo puede ser Count, Sum y Percent. |
| isTop | Booleano | Indica si el filtro es desde la parte superior o inferior |
| itemCount | Int32 | El recuento de elementos |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Dairy";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 80;
            worksheet.Cells["B4"].Value = 120;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Obtener colección de filtros pivote
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Agregar filtro Top10 - mostrar los 2 principales elementos por ventas
                PivotFilter filter = filters.AddTop10Filter(
                    baseFieldIndex: 0,          // Category field
                    valueFieldIndex: 1,          // Sales field
                    type: PivotFilterType.Count, // Filter type
                    isTop: true,                 // Show top items
                    itemCount: 2                 // Number of items to show
                );

                Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
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


