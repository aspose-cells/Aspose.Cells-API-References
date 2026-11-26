---
title: "WorkbookSettings.HidePivotFieldList"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad WorkbookSettings. Obtiene y establece si se oculta la lista de campos de la PivotTable"
type: docs
url: /es/net/aspose.cells/workbooksettings/hidepivotfieldlist/
---
## WorkbookSettings.HidePivotFieldList property

Obtiene y establece si se oculta la lista de campos para la tabla dinámica.

```csharp
public bool HidePivotFieldList { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyHidePivotFieldListDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(150);

            // Crear tabla dinámica
            int index = workbook.Worksheets.Add(SheetType.Worksheet);
            Worksheet pivotSheet = workbook.Worksheets[index];
            pivotSheet.Name = "PivotTable";
            
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:B4", "C3");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accede a la configuración del libro y establece la propiedad HidePivotFieldList
            WorkbookSettings settings = workbook.Settings;
            settings.HidePivotFieldList = true; // Hide the pivot field list

            // Guarda el libro de trabajo
            workbook.Save("HidePivotFieldListDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


