---
title: "PivotField.ShowAllItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si se deben mostrar todos los elementos en la vista de la tabla dinámica incluso si no contienen datos resumidos. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Indica si se deben mostrar todos los elementos en la vista de PivotTable, incluso si no contienen datos resumidos. El valor predeterminado es false.

```csharp
public bool ShowAllItems { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowAllItemsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Product");
            sheet.Cells["C1"].PutValue("Sales");
            
            sheet.Cells["A2"].PutValue("Electronics");
            sheet.Cells["B2"].PutValue("Laptop");
            sheet.Cells["C2"].PutValue(1200);
            
            sheet.Cells["A3"].PutValue("Electronics");
            sheet.Cells["B3"].PutValue("Phone");
            sheet.Cells["C3"].PutValue(800);
            
            sheet.Cells["A4"].PutValue("Furniture");
            sheet.Cells["B4"].PutValue("Chair");
            sheet.Cells["C4"].PutValue(150);

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Establecer la propiedad ShowAllItems para el campo de fila
            PivotField rowField = pivotTable.RowFields[0];
            rowField.ShowAllItems = true;

            // Calcular datos y guardar
            pivotTable.CalculateData();
            workbook.Save("PivotFieldShowAllItemsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


