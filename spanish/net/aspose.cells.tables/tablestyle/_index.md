---
title: "Clase TableStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Tables.TableStyle. Representa el estilo de la tabla"
type: docs
url: /es/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Representa el estilo de la tabla.

```csharp
public class TableStyle
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Obtiene el nombre del estilo de tabla. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Obtiene todos los elementos del estilo de tabla. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | Crea un estilo de tabla/tabla dinámica vacío. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleDemo
    {
        public static void TableStyleExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear estilos para la primera y última columnas
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Definir un nombre de estilo de tabla personalizado
            string tableStyleName = "Custom1";

            // Acceder a la colección de estilos de tabla
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Agregar un nuevo estilo de tabla a la colección
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Acceder a la colección de elementos del estilo de tabla
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Agregar y establecer el estilo para la primera columna
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Agregar y establecer el estilo para la última columna
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Accede a las celdas de la primera hoja de cálculo
            Cells cells = workbook.Worksheets[0].Cells;

            // Rellena la primera fila con los nombres de columna
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Rellena el resto de las celdas con datos de ejemplo
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Agregar una tabla a la hoja de cálculo
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Aplicar el estilo de tabla personalizado a la tabla
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Guarda el libro de trabajo
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


