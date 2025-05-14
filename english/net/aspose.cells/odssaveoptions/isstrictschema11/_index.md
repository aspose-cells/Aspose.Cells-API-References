---
title: OdsSaveOptions.IsStrictSchema11
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions property. Indicates whether the ods file should be saved as ODF format version 1.1. Default is false
type: docs
url: /net/aspose.cells/odssaveoptions/isstrictschema11/
---
## OdsSaveOptions.IsStrictSchema11 property

Indicates whether the ods file should be saved as ODF format version 1.1. Default is false.

```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use OdsSaveOptions.OdfStrictVersion property. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: saveOptions.IsStrictSchema11 = true;
public static void OdsSaveOptions_Property_IsStrictSchema11()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Create an instance of OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Setting properties
            saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
            saveOptions.IsStrictSchema11 = true;
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the workbook as ODS file with the specified options
            workbook.Save("OdsSaveOptionsExample.ods", saveOptions);

            return;
        }
```

### See Also

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


