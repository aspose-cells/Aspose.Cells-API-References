---
title: "TableStyleElement.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TableStyleElement. Obtiene el tipo del elemento"
type: docs
url: /es/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

Obtiene el tipo de elemento.

```csharp
public TableStyleElementType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crear una tabla
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Obtener el estilo de tabla (usando el nombre del estilo en lugar de crear uno nuevo)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // Acceder a los elementos de estilo de tabla
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // Mostrar el tipo actual del elemento
            Console.WriteLine("Current Type value: " + element.Type);

            // Nota: la propiedad Type es de solo lectura, por lo que no podemos establecerla
            // element.Type = TableStyleElementType.TotalRow; // Esto causaría un error de compilación

            // Demostrar cómo diferentes tipos de elemento afectan la tabla
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


