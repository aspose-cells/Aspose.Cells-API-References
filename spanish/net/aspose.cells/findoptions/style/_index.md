---
title: "FindOptions.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. El formato a buscar"
type: docs
url: /es/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

El formato a buscar.

```csharp
public Style Style { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con fuente azul
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // Aplicar el estilo a la celda F2
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // Crear opciones de búsqueda con el estilo
            FindOptions options = new FindOptions();
            options.Style = style;

            // Encontrar la celda con estilo coincidente
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // Mostrar el nombre de la celda encontrada
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


