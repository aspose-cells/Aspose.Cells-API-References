---
title: "Enumeración OpenDocumentFormatVersionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. Tipo de versión de Open Document Format"
type: docs
url: /es/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Tipo de versión del Formato de Documento Abierto.

```csharp
public enum OpenDocumentFormatVersionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Ninguno estricto. |
| Odf11 | `1` | Versión ODF 1.1 |
| Odf12 | `2` | Versión ODF 1.2 |
| Odf13 | `3` | Versión ODF 1.3 |
| Odf14 | `4` | Versión ODF 1.4 |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OpenDocumentFormatVersionTypeDemo
    {
        public static void OpenDocumentFormatVersionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Cree OdsSaveOptions y establezca la versión ODF
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Guarde el libro de trabajo en formato ODS con la versión ODF especificada
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


