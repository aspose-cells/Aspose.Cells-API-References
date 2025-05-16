---
title: Workbook.ExportXml
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Export XML data linked by the specified XML map
type: docs
url: /net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Export XML data linked by the specified XML map.

```csharp
public void ExportXml(string mapName, string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| path | String | the export path |

### Examples

The following code exported the data linked by the first XmlMap.

```csharp
Workbook wb = new Workbook("Book1.xlsx");

//Make sure that the source xlsx file contains a XmlMap.
XmlMap xmlMap = wb.Worksheets.XmlMaps[0];

wb.ExportXml(xmlMap.Name, "output.xml");
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Export XML data.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| stream | Stream | the export stream |

### Examples

```csharp
namespace AsposeCellsExamples.WorkbookMethodExportXmlWithStringStreamDemo
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodExportXmlWithStringStreamDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Create a memory stream to hold the XML data
            using (MemoryStream xmlStream = new MemoryStream())
            {
                try
                {
                    // Call ExportXml with mapName and stream parameters
                    workbook.ExportXml("SampleMap", xmlStream);

                    // Reset stream position to read the content
                    xmlStream.Position = 0;

                    // Read the XML content from the stream
                    using (StreamReader reader = new StreamReader(xmlStream))
                    {
                        string xmlContent = reader.ReadToEnd();
                        Console.WriteLine("Exported XML content:");
                        Console.WriteLine(xmlContent);
                    }

                    Console.WriteLine("ExportXml method executed successfully with parameters (String, Stream)");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing ExportXml method: {ex.Message}");
                }
            }

            // Save the workbook
            workbook.Save("WorkbookMethodExportXmlWithStringStreamDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


