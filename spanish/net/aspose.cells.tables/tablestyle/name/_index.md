---
title: "TableStyle.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "TableStyle property. Obtiene el nombre del estilo de tabla"
type: docs
url: /es/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Obtiene el nombre del estilo de tabla.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la colección de estilos de tabla
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Obtener el primer estilo de tabla de la colección
                TableStyle tableStyle = tableStyles[0];

                // Mostrar el valor de la propiedad Name
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Demostrar el acceso a la propiedad de solo lectura
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Mostrar que podemos usar el nombre para referenciar el estilo
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Guarda el libro de trabajo
                workbook.Save("TableStyleNameDemo.xlsx");
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

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


