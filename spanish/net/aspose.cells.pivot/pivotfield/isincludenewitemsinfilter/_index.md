---
title: "PivotField.IsIncludeNewItemsInFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si se deben incluir nuevos elementos al campo en un filtro manual. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/
---
## PivotField.IsIncludeNewItemsInFilter property

Indica si se deben incluir nuevos elementos al campo en el filtro manual. El valor predeterminado es false.

```csharp
public bool IsIncludeNewItemsInFilter { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsIncludeNewItemsInFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtener el campo dinámico y establecer IsIncludeNewItemsInFilter
            PivotField field = pivotTable.RowFields[0];
            field.IsIncludeNewItemsInFilter = true;
            
            // Mostrar el valor de la propiedad
            Console.WriteLine("IsIncludeNewItemsInFilter: " + field.IsIncludeNewItemsInFilter);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldPropertyIsIncludeNewItemsInFilterDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


