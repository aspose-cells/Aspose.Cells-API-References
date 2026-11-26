---
title: "PivotFieldSortSetting.SortType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldSortSetting. Representa el SortOrder"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsortsetting/sorttype/
---
## PivotFieldSortSetting.SortType property

Representa el [`SortOrder`](../../../aspose.cells/sortorder/).

```csharp
public SortOrder SortType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertySortTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
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
            
            // Ordenar el campo de fila en orden ascendente
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E5");
            
            // Demostrar la propiedad SortType
            Console.WriteLine("Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Cambiar el orden de clasificación y demostrar nuevamente
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "E6");
            Console.WriteLine("Updated Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Updated sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
        }
    }
}
```

### Ver también

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


