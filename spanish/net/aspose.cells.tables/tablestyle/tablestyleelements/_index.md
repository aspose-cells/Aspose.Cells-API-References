---
title: "TableStyle.TableStyleElements"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "TableStyle property. Obtiene todos los elementos del estilo de tabla"
type: docs
url: /es/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Obtiene todos los elementos del estilo de tabla.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStylePropertyTableStyleElementsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo para la tabla
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear una tabla
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // Obtener el estilo de tabla (usar un estilo existente en lugar de crear uno nuevo)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // Modificar los elementos del estilo de tabla
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // Aplicar el estilo modificado a la tabla
            table.TableStyleName = style.Name;

            // Guarda el libro de trabajo
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


