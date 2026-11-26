---
title: "TableStyleCollection.AddTableStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "TableStyleCollection method. Añade un estilo de tabla personalizado"
type: docs
url: /es/net/aspose.cells.tables/tablestylecollection/addtablestyle/
---
## TableStyleCollection.AddTableStyle method

Agrega un estilo de tabla personalizado.

```csharp
public int AddTableStyle(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del estilo de tabla. |

### Valor de retorno

El índice del estilo de tabla.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionMethodAddTableStyleWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue("Header " + (i + 1));
                for (int row = 1; row < 6; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Crear un estilo de tabla personalizado
            string styleName = "MyCustomStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Aplicar estilo a la fila de encabezado
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            headerStyle.Pattern = BackgroundType.Solid;

            tableStyle.TableStyleElements.Add(TableStyleElementType.HeaderRow);
            TableStyleElement headerElement = tableStyle.TableStyleElements[TableStyleElementType.HeaderRow];
            headerElement.SetElementStyle(headerStyle);

            // Aplicar estilo a la primera columna
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Font.Color = System.Drawing.Color.Red;

            tableStyle.TableStyleElements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement firstColElement = tableStyle.TableStyleElements[TableStyleElementType.FirstColumn];
            firstColElement.SetElementStyle(firstColStyle);

            // Crear una tabla con el estilo personalizado
            int tableIndex = worksheet.ListObjects.Add(0, 0, 5, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleName = styleName;
            table.ShowTableStyleFirstColumn = true;

            workbook.Save("CustomTableStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


