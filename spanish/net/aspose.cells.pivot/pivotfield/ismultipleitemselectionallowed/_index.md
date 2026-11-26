---
title: "PivotField.IsMultipleItemSelectionAllowed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si se pueden seleccionar múltiples elementos en el campo de página. El valor predeterminado es false."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/
---
## PivotField.IsMultipleItemSelectionAllowed property

Indica si se pueden seleccionar varios elementos en el campo de página. El valor predeterminado es false.

```csharp
public bool IsMultipleItemSelectionAllowed { get; set; }
```

### Observaciones

Solo para campos de página (filtro).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsMultipleItemSelectionAllowedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Acceda al campo de página y establezca la selección múltiple
            PivotField pageField = pivotTable.PageFields[0];
            pageField.IsMultipleItemSelectionAllowed = true;
            
            // Verificar que la propiedad se haya establecido
            Console.WriteLine("IsMultipleItemSelectionAllowed: " + pageField.IsMultipleItemSelectionAllowed);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldIsMultipleItemSelectionAllowedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


