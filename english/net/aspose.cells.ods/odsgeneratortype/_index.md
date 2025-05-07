---
title: Enum OdsGeneratorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Ods.OdsGeneratorType enum. Represents the type of ODS generator
type: docs
url: /net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

Represents the type of ODS generator.

```csharp
public enum OdsGeneratorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Examples

```csharp
// Called: saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
public static void Type_OdsGeneratorType()
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

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


