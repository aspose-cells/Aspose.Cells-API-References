---
title: "TableStyleElement.GetElementStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TableStyleElement. Obtiene el estilo del elemento"
type: docs
url: /es/net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

Obtiene el estilo del elemento.

```csharp
public Style GetElementStyle()
```

### Valor de retorno

Devuelve el objeto [`Style`](../../../aspose.cells/style/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementMethodGetElementStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Crear una tabla
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Obtener el estilo de tabla de la colección de estilos de tabla del libro de trabajo
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            TableStyle style = tableStyles[0];
            table.TableStyleName = style.Name;
            
            // Acceder al elemento completo de estilo de tabla
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
            
            // Obtener el estilo del elemento
            Style tableStyle = element.GetElementStyle();
            
            // Modificar las propiedades del estilo
            tableStyle.Font.Name = "Arial";
            tableStyle.Font.Size = 12;
            tableStyle.Font.IsBold = true;
            tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            
            // Restablecer el estilo modificado
            element.SetElementStyle(tableStyle);
            
            // Guarda el libro de trabajo
            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


