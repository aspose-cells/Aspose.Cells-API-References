---
title: OdsSaveOptions.OdsSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions constructor. Creates the options of saving ods file
type: docs
url: /net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Creates the options of saving ods file.

```csharp
public OdsSaveOptions()
```

### Examples

```csharp
// Called: OdsSaveOptions saveOptions = new OdsSaveOptions();
public static void OdsSaveOptions_Constructor()
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

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Creates the options of saving ods file.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Ods, Ots, Fods or Sxc, otherwise the saved format will be set as Ods automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


