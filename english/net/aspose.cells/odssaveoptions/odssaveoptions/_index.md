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
public void OdsSaveOptions_Constructor()
{
    Style style = null;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    OdsSaveOptions saveOptions = new OdsSaveOptions();
    saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
    workbook.Save(Constants.destPath + "example.ods", saveOptions);
    workbook = new Workbook(Constants.destPath + "example.ods");
    style = workbook.Worksheets[0].Cells["B2"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
    style = workbook.Worksheets[0].Cells["B4"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
    style = workbook.Worksheets[0].Cells["B7"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    style = workbook.Worksheets[0].Cells["B2"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
    style = workbook.Worksheets[0].Cells["B4"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
    style = workbook.Worksheets[0].Cells["B7"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
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

### Examples

```csharp
namespace AsposeCellsExamples.OdsSaveOptionsMethodCtorWithSaveFormatDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Call the #ctor method with SaveFormat parameter
                OdsSaveOptions saveOptions = new OdsSaveOptions(SaveFormat.Ods);
                
                // Set some properties of the save options
                saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
                saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
                
                Console.WriteLine("OdsSaveOptions constructor executed successfully with SaveFormat.Ods parameter");
                
                // Save the workbook with the specified options
                workbook.Save("OdsSaveOptionsCtorDemo.ods", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OdsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


