---
title: XmlSaveOptions.HasHeaderRow
second_title: Aspose.Cells for .NET API Reference
description: XmlSaveOptions property. Indicates whether the range contains header row
type: docs
url: /net/aspose.cells/xmlsaveoptions/hasheaderrow/
---
## XmlSaveOptions.HasHeaderRow property

Indicates whether the range contains header row.

```csharp
public bool HasHeaderRow { get; set; }
```

### Examples

```csharp
// Called: saveOptions.HasHeaderRow = true;
public static void XmlSaveOptions_Property_HasHeaderRow()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data in the worksheet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Create an instance of XmlSaveOptions
            XmlSaveOptions saveOptions = new XmlSaveOptions();

            // Setting properties
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 };
            saveOptions.HasHeaderRow = true;
            saveOptions.XmlMapName = "MyXmlMap";
            saveOptions.SheetNameAsElementName = true;
            saveOptions.DataAsAttribute = false;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the workbook as an XML file
            workbook.Save("XmlSaveOptionsExample.xml", saveOptions);

            return;
        }
```

### See Also

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


