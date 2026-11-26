---
title: "Style.IsJustifyDistributed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si se debe usar alineación justificada o distribuida en la última línea de texto de las celdas"
type: docs
url: /es/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Indica si la alineación justificada o distribuida de las celdas debe usarse en la última línea de texto.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Observaciones

Esto es típico para alineaciones de Asia Oriental pero no es típico en otros contextos. Solo funciona cuando la alineación distribuida horizontal está activada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda B3 y establecer su texto
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // Obtener el estilo de la celda y establecer IsJustifyDistributed a true
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Verificar la propiedad
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


