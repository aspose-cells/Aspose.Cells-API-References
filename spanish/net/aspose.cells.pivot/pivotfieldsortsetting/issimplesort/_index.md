---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldSortSetting. Indica si se aplicará una operación de ordenación de datos simple"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

Indica si se aplicará una operación simple de ordenación de datos.

```csharp
public bool IsSimpleSort { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtener campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // Obtener configuración de ordenación (propiedad de solo lectura)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Mostrar valor actual de IsSimpleSort
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // Nota: IsSimpleSort es de solo lectura, por lo que no podemos establecerlo directamente
            // Para demostrar la ordenación, crearemos una nueva tabla dinámica con una ordenación diferente

            // Crear otra tabla dinámica con ordenación personalizada
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ordenar el campo dinámico usando el método disponible
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


