---
title: "PivotField.FilterByLabel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotField. Filtra por los títulos de los campos pivot de fila o columna"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

Filtra por los títulos del campo pivot de fila o columna.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | PivotFilterType | El tipo de datos de filtrado. |
| label1 | String | La etiqueta de la condición de filtro |
| label2 | String | La etiqueta límite superior de la condición de filtro entre |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Crea una tabla dinámica con los parámetros correctos
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Obtener el campo de pivote
            PivotField field = pivot.RowFields[0];
            
            // Aplicar filtros
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFilterByLabelDemo.xlsx");
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


