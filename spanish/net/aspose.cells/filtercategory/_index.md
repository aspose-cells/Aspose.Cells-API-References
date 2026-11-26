---
title: "Enumeración FilterCategory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.FilterCategory. Representa la categoría del filtro"
type: docs
url: /es/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

Representa la categoría del filtro.

```csharp
public enum FilterCategory
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin filtro. |
| Label | `1` | Filtro de título. |
| NumberValue | `2` | Filtro de valor numérico. |
| Date | `3` | Filtro de valor de fecha. |
| Top10 | `4` | Filtro Top10 de valor. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            CreateSampleData(worksheet);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configurar campos de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // Configurar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Agregar filtro de etiqueta a los filtros de tabla dinámica
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // Demostrar el uso de FilterCategory
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // Mostrar todas las categorías de filtro en la tabla dinámica
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guardar el resultado
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Establecer encabezados de datos de muestra
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // Agregar filas de datos de muestra
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


