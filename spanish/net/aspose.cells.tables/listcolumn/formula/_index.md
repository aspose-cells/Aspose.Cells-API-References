---
title: "ListColumn.Formula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListColumn. Obtiene y establece la fórmula de la columna de lista"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Obtiene y establece la fórmula de la columna de lista.

```csharp
public string Formula { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Cree datos de ejemplo y tabla
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["A3"].PutValue(10);
            sheet.Cells["A4"].PutValue(15);
            
            sheet.Cells["B1"].PutValue("Doubled");
            sheet.Cells["B2"].PutValue("=A2*2");
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            
            // Agregue la fórmula a la columna de lista
            ListColumn column = table.ListColumns[0];
            column.Formula = "=A2*3"; // This will apply to all cells in the column
            
            // Guarda el libro de trabajo
            workbook.Save("ListColumnFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


