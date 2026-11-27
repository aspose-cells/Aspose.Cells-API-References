---
title: "Enum OpenDocumentFormatVersionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType-enum. Open Document Format versionstyp"
type: docs
url: /sv/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Open Document Format versionstyp.

```csharp
public enum OpenDocumentFormatVersionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen strikt. |
| Odf11 | `1` | ODF Version 1.1 |
| Odf12 | `2` | ODF Version 1.2 |
| Odf13 | `3` | ODF Version 1.3 |
| Odf14 | `4` | ODF Version 1.4 |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Skapa OdsSaveOptions och ange ODF-versionen
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Spara arbetsboken i ODS-format med den angivna ODF-versionen
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


