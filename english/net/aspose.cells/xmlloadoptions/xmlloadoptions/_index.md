---
title: XmlLoadOptions.XmlLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions constructor. Represents the options of loading xml file
type: docs
url: /net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Represents the options of loading xml file.

```csharp
public XmlLoadOptions()
```

### Examples

```csharp
// Called: XmlLoadOptions options = new XmlLoadOptions();
public void XmlLoadOptions_Constructor()
{
    bool[] flags = {true, false};
    foreach(bool flag in flags)
    {
        XmlLoadOptions options = new XmlLoadOptions();
        options.ConvertNumericOrDate = flag;
        Workbook wb = new Workbook(Constants.sourcePath + "example.xml", options);
        // wb.Worksheets.RefreshAll();
        Cell cell = wb.Worksheets[0].Cells["E4"];
       Assert.IsTrue( (cell.Type == CellValueType.IsString) != flag);
        wb.Save(Constants.destPath + "example.xlsx");
    }
            
}
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Represents the options of loading xml file.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | LoadFormat | The load format type. |

### Examples

```csharp
namespace AsposeCellsExamples.XmlLoadOptionsMethodCtorWithLoadFormatDemo
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Create XmlLoadOptions instance with LoadFormat parameter
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // Set some properties of the XmlLoadOptions
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Create a workbook using the load options
                Workbook workbook = new Workbook("input.xml", xmlLoadOptions);

                // Access the first worksheet
                Worksheet worksheet = workbook.Worksheets[0];

                // Display some information
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Save the workbook
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


