---
title: "PivotField.IsInsertPageBreaksBetweenItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotField. Indica si se deben insertar saltos de página después de cada elemento. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/
---
## PivotField.IsInsertPageBreaksBetweenItems property

Indica si se deben insertar saltos de página después de cada elemento. El valor predeterminado es false.

```csharp
public bool IsInsertPageBreaksBetweenItems { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsInsertPageBreaksBetweenItemsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 7; i++)
            {
                worksheet.Cells["A" + i].PutValue("Category " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Verificar el recuento de páginas antes de establecer la propiedad
            SheetRender render1 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count before: " + render1.PageCount);

            // Establecer la propiedad IsInsertPageBreaksBetweenItems
            PivotField field = pivotTable.RowFields[0];
            field.IsInsertPageBreaksBetweenItems = true;
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Verificar el recuento de páginas después de establecer la propiedad
            SheetRender render2 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count after: " + render2.PageCount);

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldIsInsertPageBreaksBetweenItemsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


