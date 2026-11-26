---
title: "Enumeración TableStyleElementType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Tables.TableStyleElementType. Representa el tipo de elemento de estilo de tabla o tabla dinámica"
type: docs
url: /es/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Representa el tipo de elemento de estilo de Tabla o Tabla dinámica.

```csharp
public enum TableStyleElementType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| BlankRow | `18` | Elemento de estilo de tabla que se aplica a las filas en blanco de la tabla dinámica. |
| FirstColumn | `8` | Elemento de estilo de tabla que se aplica a la primera columna de la tabla. |
| FirstColumnStripe | `3` | Elemento de estilo de tabla que se aplica a las franjas de la primera columna de la tabla. |
| FirstColumnSubheading | `22` | Elemento de estilo de tabla que se aplica al subtítulo de la primera columna de la tabla dinámica. |
| FirstHeaderCell | `11` | Elemento de estilo de tabla que se aplica a la primera celda de la fila de encabezado de la tabla. |
| FirstRowStripe | `5` | Elemento de estilo de tabla que se aplica a las franjas de la primera fila de la tabla. |
| FirstRowSubheading | `25` | Elemento de estilo de tabla que se aplica al subtítulo de la primera fila de la tabla dinámica. |
| FirstSubtotalColumn | `15` | Elemento de estilo de tabla que se aplica a la primera columna de subtotal de la tabla dinámica. |
| FirstSubtotalRow | `19` | Elemento de estilo de tabla que se aplica a la primera fila de subtotal de la tabla dinámica. |
| GrandTotalColumn | `28` | Elemento de estilo de tabla que se aplica a la columna de total general de la tabla dinámica. |
| GrandTotalRow | `29` | Elemento de estilo de tabla que se aplica a la fila de total general de la tabla dinámica. |
| FirstTotalCell | `13` | Elemento de estilo de tabla que se aplica a la primera celda de la fila de total de la tabla. |
| HeaderRow | `9` | Elemento de estilo de tabla que se aplica a la fila de encabezado de la tabla. |
| LastColumn | `7` | Elemento de estilo de tabla que se aplica a la última columna de la tabla. |
| LastHeaderCell | `12` | Elemento de estilo de tabla que se aplica a la última celda de la fila de encabezado de la tabla. |
| LastTotalCell | `14` | Elemento de estilo de tabla que se aplica a la última celda de la fila de total de la tabla. |
| PageFieldLabels | `1` | Elemento de estilo de tabla que se aplica a las etiquetas de campo de página de la tabla dinámica. |
| PageFieldValues | `2` | Elemento de estilo de tabla que se aplica a los valores del campo de página de la tabla dinámica. |
| SecondColumnStripe | `4` | Elemento de estilo de tabla que se aplica a las franjas de la segunda columna de la tabla. |
| SecondColumnSubheading | `23` | Elemento de estilo de tabla que se aplica al subtítulo de la segunda columna de la tabla dinámica. |
| SecondRowStripe | `6` | Elemento de estilo de tabla que se aplica a las franjas de la segunda fila de la tabla. |
| SecondRowSubheading | `26` | Elemento de estilo de tabla que se aplica al subtítulo de la segunda fila de la tabla dinámica. |
| SecondSubtotalColumn | `16` | Elemento de estilo de tabla que se aplica a la segunda columna de subtotal de la tabla dinámica. |
| SecondSubtotalRow | `20` | Elemento de estilo de tabla que se aplica a la segunda fila de subtotal de la tabla dinámica. |
| ThirdColumnSubheading | `24` | Elemento de estilo de tabla que se aplica al subtítulo de la tercera columna de la tabla dinámica. |
| ThirdRowSubheading | `27` | Elemento de estilo de tabla que se aplica al subtítulo de la tercera fila de la tabla dinámica. |
| ThirdSubtotalColumn | `17` | Elemento de estilo de tabla que se aplica a la tercera columna de subtotal de la tabla dinámica. |
| ThirdSubtotalRow | `21` | Elemento de estilo de tabla que se aplica a la tercera fila de subtotal de la tabla dinámica. |
| TotalRow | `10` | Elemento de estilo de tabla que se aplica a la fila total de la tabla. |
| WholeTable | `0` | Elemento de estilo de tabla que se aplica a todo el contenido de la tabla. |
| LastColumnSubheading | `130` | Elemento de estilo de tabla que se aplica al último campo de columna de la tabla dinámica. |
| LastRowSubheading | `131` | Elemento de estilo de tabla que se aplica al último campo de fila de la tabla dinámica. |
| LastSubtotalRow | `133` | Elemento de estilo de tabla que se aplica al último campo de fila de subtotal de la tabla dinámica. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleElementTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            
            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.ForegroundColor = System.Drawing.Color.LightGreen;

            string tableStyleName = "CustomStyle1";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            elements[elementIndex].SetElementStyle(firstColumnStyle);
            
            elementIndex = elements.Add(TableStyleElementType.LastColumn);
            elements[elementIndex].SetElementStyle(lastColumnStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue($"Column {i + 1}");
            }

            for (int row = 1; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue(row * col);
                }
            }

            ListObject table = workbook.Worksheets[0].ListObjects[workbook.Worksheets[0].ListObjects.Add(0, 0, 4, 4, true)];
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


