---
title: "Enumeración TextCapsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.TextCapsType. Este tipo especifica los tipos de mayúsculas del texto"
type: docs
url: /es/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

Este tipo especifica los tipos de mayúsculas del texto.

```csharp
public enum TextCapsType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin mayúsculas |
| All | `1` | Aplicar todas las mayúsculas al texto. |
| Small | `2` | Aplicar versalitas al texto. |

### Observaciones

Solo se puede aplicar a gráficos y formas.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Código adicional para demostrar cómo se podría usar la instancia
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el valor de una celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Obtener el estilo de la celda
            Style style = cell.GetStyle();

            // Establecer el tipo de mayúsculas de la fuente a Todas las mayúsculas
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Aplique el estilo a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


