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

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Create a workbook and load the Excel file
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Get the first XmlMap from the workbook
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Export XML data using the XmlMap's name and output file path
                wb.ExportXml(xmlMap.Name, "output.xml");
                Console.WriteLine("XML exported successfully to output.xml");
            }
            else
            {
                Console.WriteLine("No XmlMap found in the workbook");
            }
        }
    }
}
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
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStreamDemo
    {
        public static void Run()
        {
            // Create a new workbook and add some data
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Name of the XML map to export – for demo purposes we use a placeholder name
                string mapName = "SampleMap";

                try
                {
                    // Export the XML map to a file using a FileStream (String, Stream overload)
                    string outputPath = "ExportedSample.xml";
                    using (FileStream fs = new FileStream(outputPath, FileMode.Create, FileAccess.Write))
                    {
                        workbook.ExportXml(mapName, fs);
                    }

                    Console.WriteLine($"ExportXml completed successfully. Output saved to '{outputPath}'.");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during ExportXml: {ex.Message}");
                }
            }
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


