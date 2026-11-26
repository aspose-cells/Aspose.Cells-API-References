---
title: "Clase PivotFieldSortSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting class. Representa la configuración para ordenar campos de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Representa la configuración para ordenar los campos de tabla dinámica.

```csharp
public class PivotFieldSortSetting
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Ordena por los valores en la fila o columna. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Obsoleto.**) Representa el índice del campo por el cual se ordena. -1 significa ordenar el PivotField por las etiquetas, otros significa ordenar por el campo de datos. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | Indica si se aplicará una operación simple de ordenación de datos. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Indica si se debe ordenar el campo por sí mismo o por el campo de datos. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | El tipo de línea de pivote ordenado por. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | Representa el índice del campo por el cual se ordena. Un valor de -1 indica ordenación por los propios valores del elemento de pivote. Cuando es mayor o igual a cero, representa el índice del campo de datos en la región de datos. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | Representa el [`SortOrder`](../../aspose.cells/sortorder/). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtener la configuración de ordenación del campo de pivote de la tabla dinámica
            // Nota: Esto asume que la tabla dinámica tiene configuraciones de ordenación a las que podemos acceder
            // Dado que no podemos crear un nuevo PivotFieldSortSetting directamente
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Propiedades de visualización (solo lectura)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Aplicar ordenación a la tabla dinámica (la ordenación real se realizará mediante los métodos de la tabla dinámica)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guardar el resultado
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


