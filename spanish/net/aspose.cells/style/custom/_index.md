---
title: "Style.Custom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Representa la cadena de formato numérico personalizado de este objeto de estilo. Si el formato numérico personalizado no está establecido, por ejemplo, se devolverá el formato numérico incorporado"
type: docs
url: /es/net/aspose.cells/style/custom/
---
## Style.Custom property

Representa la cadena de formato numérico personalizado de este objeto de estilo. Si el formato numérico personalizado no está establecido (Por ejemplo, el formato numérico es incorporado), se devolverá "".

```csharp
public string Custom { get; set; }
```

### Observaciones

La cadena personalizada devuelta es independiente de la cultura.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCustomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear y aplicar un formato de fecha personalizado
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // Mostrar el valor formateado
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // Guarda el libro de trabajo
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


