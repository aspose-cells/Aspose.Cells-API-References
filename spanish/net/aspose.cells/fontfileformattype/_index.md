---
title: "Enumeración FontFileFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.FontFileFormatType enum. Representa el tipo de formato de fuente"
type: docs
url: /es/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

Representa el tipo de formato de fuente.

```csharp
public enum FontFileFormatType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Unknown | `0` | Tipo de formato de fuente desconocido. |
| Ttf | `1` | Tipo de formato de fuente TTF. |
| Otf | `2` | Tipo de formato de fuente OTF. |
| Ttc | `3` | Tipo de formato de fuente TTC. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accede a una celda y establece su estilo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // Demuestra el uso de FontFileFormatType
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // Aplica la configuración de fuente
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Verifica la compatibilidad del formato de fuente
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // Guarda el libro de trabajo
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


