---
title: "Column.HasCustomStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Column. Indica si esta columna tiene configuraciones de estilo personalizadas diferentes del estilo predeterminado heredado del libro de trabajo"
type: docs
url: /es/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

Indica si esta columna tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada del libro).

```csharp
public bool HasCustomStyle { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la primera columna
            Column column = worksheet.Cells.Columns[0];

            // Mostrar el valor inicial de HasCustomState
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // Modificar el estilo de la columna para demostrar el cambio de HasCustomStyle
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // Mostrar el valor actualizado de HasCustomStyle
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // Crear otra columna con estilo predeterminado para comparación
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // Guarda el libro de trabajo
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


