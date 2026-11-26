---
title: "PivotFilterCollection.AddLabelFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilterCollection. Filtra por los títulos del campo pivot de fila o columna"
type: docs
url: /es/net/aspose.cells.pivot/pivotfiltercollection/addlabelfilter/
---
## PivotFilterCollection.AddLabelFilter method

Filtra por los títulos del campo pivot de fila o columna.

```csharp
public PivotFilter AddLabelFilter(int baseFieldIndex, PivotFilterType type, string label1, 
    string label2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | Int32 | El índice del campo en la fuente. |
| type | PivotFilterType | El tipo de datos de filtrado. |
| label1 | String | La etiqueta de la condición de filtro |
| label2 | String | La etiqueta límite superior de la condición de filtro entre |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddLabelFilterWithInt32PivotFilterTypeStringStriDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Cherry";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

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
                
                // Agregar filtro de etiqueta para mostrar productos que comienzan con "A"
                PivotFilter filter = filters.AddLabelFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.CaptionBeginsWith,
                    label1: "A",
                    label2: null
                );

                Console.WriteLine($"Label filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value1: {filter.Value1}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding label filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddLabelFilterDemo.xlsx");
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


