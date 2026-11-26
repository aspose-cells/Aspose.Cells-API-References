---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsSaveOptions. Indica si se guardan las tablas dinámicas"
type: docs
url: /es/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

Indica si se guardan las tablas dinámicas.

```csharp
public bool IgnorePivotTables { get; set; }
```

### Observaciones

La función de tabla dinámica de OpenOffice tiene menos configuraciones en comparación con Excel, por lo que sus resultados de tabla dinámica presentan muchas diferencias. A veces es mejor ignorar estas tablas dinámicas al guardar el archivo .ods.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear una instancia de OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Mostrar el valor actual de IgnorePivotTables
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // Establecer para ignorar las tablas dinámicas al guardar
            saveOptions.IgnorePivotTables = true;

            // Guardar con las tablas dinámicas ignoradas
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // Establecer para incluir las tablas dinámicas al guardar
            saveOptions.IgnorePivotTables = false;

            // Guardar con las tablas dinámicas incluidas
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### Ver también

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


