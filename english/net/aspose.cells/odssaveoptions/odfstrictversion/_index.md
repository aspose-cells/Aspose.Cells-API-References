---
title: OdsSaveOptions.OdfStrictVersion
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions property. Gets and sets the ODF version
type: docs
url: /net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Gets and sets the ODF version.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Examples

```csharp
// Called: saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
public static void OdsSaveOptions_Property_OdfStrictVersion()
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
```

### See Also

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


