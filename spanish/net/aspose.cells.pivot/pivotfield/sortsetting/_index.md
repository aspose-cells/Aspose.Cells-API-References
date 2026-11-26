---
title: "PivotField.SortSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Obtiene todas las configuraciones de autoordenación"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/sortsetting/
---
## PivotField.SortSetting property

Obtiene todas las configuraciones de autoordenación

```csharp
public PivotFieldSortSetting SortSetting { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertySortSettingDemo
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
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 75;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];

            // Demostrar la propiedad SortSetting
            rowField.SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + rowField.SortSetting.Cell);
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);

            // Cambiar la configuración de ordenación
            rowField.SortBy(SortOrder.Descending, 0, PivotLineType.GrandTotal, null);
            Console.WriteLine("\nAfter changing sort settings:");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + (string.IsNullOrEmpty(rowField.SortSetting.Cell) ? "null" : rowField.SortSetting.Cell));
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);
        }
    }
}
```

### Ver también

* class [PivotFieldSortSetting](../../pivotfieldsortsetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


