---
title: "TableStyleElement.Size"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TableStyleElement. Número de filas o columnas en una sola banda de franjas. Se aplica solo cuando el tipo es firstRowStripe secondRowStripe firstColumnStripe o secondColumnStripe"
type: docs
url: /es/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

Número de filas o columnas en una sola banda de franjas. Se aplica solo cuando el tipo es firstRowStripe, secondRowStripe, firstColumnStripe o secondColumnStripe.

```csharp
public int Size { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crear una tabla
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Crear un estilo de tabla usando la colección de estilos del libro de trabajo
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // Agregar elementos de franjas para demostrar la propiedad Size
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // Acceder a los elementos de franjas
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // Mostrar los valores actuales de Size
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // Modificar los tamaños de las franjas
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // Mostrar los valores modificados
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


