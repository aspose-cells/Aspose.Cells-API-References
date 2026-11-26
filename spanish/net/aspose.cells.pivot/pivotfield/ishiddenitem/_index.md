---
title: "PivotField.IsHiddenItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotField. Indica si el PivotItem específico está oculto"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/ishiddenitem/
---
## PivotField.IsHiddenItem method

Indica si el PivotItem específico está oculto.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItem(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del pivotItem en el pivotField. |

### Valor de retorno

si el PivotItem específico está oculto

### Observaciones

NOTA: Este método está obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemWithInt32Demo
    {
        public static void Run()
        {
            // Crea un libro y añade datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Country";
            worksheet.Cells["A2"].Value = "USA";
            worksheet.Cells["A3"].Value = "Canada";
            worksheet.Cells["A4"].Value = "UK";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Ocultar elemento en el índice 1 (Canada)
            rowField.HideItem(1, true);
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Verificar si el elemento en el índice 1 está oculto
            bool isHidden = rowField.IsHiddenItem(1);
            Console.WriteLine("Is item at index 1 hidden? " + isHidden);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldIsHiddenItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


