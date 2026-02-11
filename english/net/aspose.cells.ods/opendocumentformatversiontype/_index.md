---
title: Enum OpenDocumentFormatVersionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. Open Document Format version type
type: docs
url: /net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Open Document Format version type.

```csharp
public enum OpenDocumentFormatVersionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | None strict. |
| Odf11 | `1` | ODF Version 1.1 |
| Odf12 | `2` | ODF Version 1.2 |
| Odf13 | `3` | ODF Version 1.3 |
| Odf14 | `4` | ODF Version 1.4 |

### Examples

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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Create OdsSaveOptions and set the ODF version
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Save the workbook in ODS format with the specified ODF version
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


