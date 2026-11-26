---
title: "PivotField.FilterTop10"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Filtra por valores del campo dinámico de datos"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

Filtra por los valores del campo pivot de datos.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valueFieldIndex | Int32 | El índice del campo de datos en la región de datos. |
| type | PivotFilterType | El tipo de filtrado de datos. Sólo puede ser Count, Sum y Percent. |
| isTop | Booleano | Indica si el filtro es desde la parte superior o inferior |
| itemCount | Int32 | El recuento de elementos |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterTop10WithInt32PivotFilterTypeBooleanIntDemo
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
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            worksheet.Cells["A7"].Value = "Banana";
            worksheet.Cells["A8"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 40;
            worksheet.Cells["B6"].Value = 50;
            worksheet.Cells["B7"].Value = 60;
            worksheet.Cells["B8"].Value = 70;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B8", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aplicar filtro top 10
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableFilterTop10.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


