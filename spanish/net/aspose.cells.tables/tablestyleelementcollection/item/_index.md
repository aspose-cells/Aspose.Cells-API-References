---
title: "TableStyleElementCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TableStyleElementCollection. Obtiene un elemento del estilo de tabla por el índice"
type: docs
url: /es/net/aspose.cells.tables/tablestyleelementcollection/item/
---
## TableStyleElementCollection indexer (1 of 2)

Obtiene un elemento del estilo de tabla por el índice.

```csharp
public TableStyleElement this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

Devuelve el objeto [`TableStyleElement`](../../tablestyleelement/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Pattern = BackgroundType.Solid;
            firstColStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[elementIndex];
            element.SetElementStyle(firstColStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data");

            int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 1, 0, true);
            ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
            table.ShowTableStyleFirstColumn = true;
            table.TableStyleName = styleName;

            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyleElement](../../tablestyleelement/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## TableStyleElementCollection indexer (2 of 2)

Obtiene el elemento del estilo de tabla por el tipo de elemento.

```csharp
public TableStyleElement this[TableStyleElementType type] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| type | El tipo de elemento. |

### Valor de retorno

Devuelve el objeto [`TableStyleElement`](../../tablestyleelement/)

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear un estilo de tabla personalizado
            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Acceder a la TableStyleElementCollection
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Agregar un elemento de estilo de tabla
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);

            try
            {
                // Acceder a la propiedad Item usando el indexador (que usa internamente la propiedad Item)
                TableStyleElement element = elements[elementIndex];

                // Mostrar información sobre el elemento
                Console.WriteLine("Table Style Element Type: " + element.Type);
                Console.WriteLine("Element has been successfully accessed via Item property");

                // Guarda el libro de trabajo
                workbook.Save("TableStyleElementItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [TableStyleElement](../../tablestyleelement/)
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


