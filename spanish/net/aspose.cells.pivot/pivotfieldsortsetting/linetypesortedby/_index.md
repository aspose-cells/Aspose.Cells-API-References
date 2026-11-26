---
title: "PivotFieldSortSetting.LineTypeSortedBy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldSortSetting. El tipo de línea dinámica por el cual se ordena"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/
---
## PivotFieldSortSetting.LineTypeSortedBy property

El tipo de línea de pivote ordenado por.

```csharp
public PivotLineType LineTypeSortedBy { get; }
```

### Observaciones

Solo funciona cuando este campo no se ordena por etiquetas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyLineTypeSortedByDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Ordenar en orden ascendente con tipo de línea - proporcionar cadena vacía para el parámetro cellName
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            
            // Demostrar la propiedad LineTypeSortedBy
            Console.WriteLine("LineTypeSortedBy: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
            
            // Cambiar orden para usar tipo de línea regular
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("LineTypeSortedBy after change: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
        }
    }
}
```

### Ver también

* enum [PivotLineType](../../pivotlinetype/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


