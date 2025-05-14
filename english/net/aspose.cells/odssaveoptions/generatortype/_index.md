---
title: OdsSaveOptions.GeneratorType
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions property. Gets and sets the generator of the ods file
type: docs
url: /net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Gets and sets the generator of the ods file.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
public static void OdsSaveOptions_Property_GeneratorType()
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

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


