---
title: "Enumeración FontSchemeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.FontSchemeType enum. Representa el tipo de esquema de la fuente"
type: docs
url: /es/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

Representa el tipo de esquema de la fuente.

```csharp
public enum FontSchemeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Ninguno |
| Major | `1` | Esquema principal. |
| Minor | `2` | Esquema secundario. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Obtenga la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            // Accediendo a la celda "A1" de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];
            // Añadiendo un valor a la celda "A1"
            cell.PutValue("Hello Aspose!");

            // Acceda a la fuente del estilo de celda
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Estableciendo el tipo de esquema de fuente a Principal
            font.SchemeType = FontSchemeType.Major;

            // Estableciendo otras propiedades de fuente para demostración
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


