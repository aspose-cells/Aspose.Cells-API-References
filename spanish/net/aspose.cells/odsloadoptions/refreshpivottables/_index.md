---
title: "OdsLoadOptions.RefreshPivotTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsLoadOptions. Indica si se deben actualizar las tablas dinámicas al cargar el archivo"
type: docs
url: /es/net/aspose.cells/odsloadoptions/refreshpivottables/
---
## OdsLoadOptions.RefreshPivotTables property

Indica si se actualizan las tablas dinámicas al cargar el archivo.

```csharp
public bool RefreshPivotTables { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con tabla dinámica
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["C1"].PutValue("Price");
            sheet.Cells["C2"].PutValue(2.5);
            sheet.Cells["C3"].PutValue(3.0);
            sheet.Cells["C4"].PutValue(1.5);

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");

            // Guardar como ODS
            string odsPath = "output.ods";
            wb.Save(odsPath, SaveFormat.Ods);

            // Cargar con RefreshPivotTables habilitado
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;
            Workbook wb2 = new Workbook(odsPath, loadOptions);

            // Verificar que la tabla dinámica se actualizó
            Console.WriteLine("Pivot table count: " + wb2.Worksheets[0].PivotTables.Count);
        }
    }
}
```

### Ver también

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


