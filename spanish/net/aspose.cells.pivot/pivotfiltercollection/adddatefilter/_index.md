---
title: "PivotFilterCollection.AddDateFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilterCollection. Filtra por la configuración de fecha de la fila o columna del campo pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotfiltercollection/adddatefilter/
---
## PivotFilterCollection.AddDateFilter method

Filtra por la configuración de fecha del campo pivot de fila o columna.

```csharp
public PivotFilter AddDateFilter(int baseFieldIndex, PivotFilterType type, DateTime dateTime1, 
    DateTime dateTime2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | Int32 | El índice del campo en la fuente. |
| type | PivotFilterType | El tipo de datos de filtrado. |
| dateTime1 | DateTime | La etiqueta de fecha de la condición de filtro |
| dateTime2 | DateTime | La etiqueta de fecha límite superior de la condición de filtro entre |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddDateFilterWithInt32PivotFilterTypeDateTimeDaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con fechas
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

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
                
                // Agregar filtro de fecha para mostrar fechas entre el 1 de enero y el 31 de marzo de 2023
                PivotFilter filter = filters.AddDateFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.DateBetween,
                    dateTime1: new DateTime(2023, 1, 1),
                    dateTime2: new DateTime(2023, 3, 31)
                );

                Console.WriteLine($"Date filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, UseWholeDay: {filter.UseWholeDay}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding date filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddDateFilterDemo.xlsx");
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


