---
title: XmlSaveOptions.SheetNameAsElementName
second_title: Aspose.Cells for .NET API Reference
description: XmlSaveOptions property. Indicates whether exporting sheets name as the name of the element
type: docs
url: /net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

Indicates whether exporting sheet's name as the name of the element.

```csharp
public bool SheetNameAsElementName { get; set; }
```

### Examples

```csharp
// Called: saveOptions.SheetNameAsElementName = true;
public static void Property_SheetNameAsElementName()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data in the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Header1&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Header2&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Data1&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(&quot;Data2&quot;);

            // Create an instance of XmlSaveOptions
            XmlSaveOptions saveOptions = new XmlSaveOptions();

            // Setting properties
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 };
            saveOptions.HasHeaderRow = true;
            saveOptions.XmlMapName = &quot;MyXmlMap&quot;;
            saveOptions.SheetNameAsElementName = true;
            saveOptions.DataAsAttribute = false;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = &quot;C:\\Temp&quot;;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the workbook as an XML file
            workbook.Save(&quot;XmlSaveOptionsExample.xml&quot;, saveOptions);

            return;
        }
```

### See Also

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


