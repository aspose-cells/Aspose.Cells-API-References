---
title: "Worksheet.RefreshPivotTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Actualiza todas las PivotTables en esta Worksheet"
type: docs
url: /es/net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Actualiza todas las PivotTables en esta hoja de cálculo.

```csharp
public void RefreshPivotTables()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente que contiene tablas dinámicas
            Workbook workbook = new Workbook("example.xlsx");
            
            // Obtener la primera hoja de cálculo que contiene tablas dinámicas
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Actualizar todas las tablas dinámicas en la hoja de cálculo
            worksheet.RefreshPivotTables();
            
            // Guardar el libro de trabajo actualizado
            workbook.Save("RefreshedPivotTables.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Actualiza todas las PivotTables en esta hoja de cálculo.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opción | PivotTableRefreshOption | La opción para actualizar la fuente de datos de la tabla dinámica. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
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
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            worksheet.RefreshPivotTables();

            int preCount = pivotTable.RowFields[0].PivotItems.Count;


            // Modificar los datos de origen
            worksheet.Cells["A2"].Value = "test2";
            worksheet.Cells["A3"].Value = "test3";

            // Crear opciones de actualización
            PivotTableRefreshOption options = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
            };
            worksheet.RefreshPivotTables(options);
            int nowCount = pivotTable.RowFields[0].PivotItems.Count;
            Console.WriteLine(nowCount > preCount);
                        

            // Guardar el resultado
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


