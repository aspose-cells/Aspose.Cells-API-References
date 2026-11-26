---
title: "PivotAreaFilter.IsSubtotalSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotAreaFilter. Obtiene qué subtotal está configurado para este filtro"
type: docs
url: /es/net/aspose.cells.pivot/pivotareafilter/issubtotalset/
---
## PivotAreaFilter.IsSubtotalSet method

Obtiene qué subtotal está configurado para este filtro.

```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | El tipo de función de subtotal. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterMethodIsSubtotalSetWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila y configurar subtotales
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;
            rowField.SetSubtotals(PivotFieldSubtotalType.Automatic, true);

            // Crear área de tabla dinámica y comprobar la configuración del subtotal
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            
            // Demostrar el uso de IsSubtotalSet
            bool isSubtotalSet = pivotArea.Filters[0].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            Console.WriteLine($"Is Automatic subtotal set: {isSubtotalSet}");

            // Guarda el libro de trabajo
            workbook.Save("PivotSubtotalDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


