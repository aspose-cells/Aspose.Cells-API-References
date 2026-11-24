---
title: "Enum OpenDocumentFormatVersionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. Typ der Open Document Format-Version"
type: docs
url: /de/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Open Document Format Versions­typ.

```csharp
public enum OpenDocumentFormatVersionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine strenge. |
| Odf11 | `1` | ODF Version 1.1 |
| Odf12 | `2` | ODF Version 1.2 |
| Odf13 | `3` | ODF Version 1.3 |
| Odf14 | `4` | ODF Version 1.4 |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Erstellen Sie OdsSaveOptions und setzen Sie die ODF-Version
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Speichern Sie die Arbeitsmappe im ODS-Format mit der angegebenen ODF-Version
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


