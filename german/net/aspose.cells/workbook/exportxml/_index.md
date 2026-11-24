---
title: "Workbook.ExportXml"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Exportieren von XML-Daten, die mit der angegebenen XML-Map verknüpft sind"
type: docs
url: /de/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Exportiert XML‑Daten, die durch die angegebene XML‑Zuordnung verknüpft sind.

```csharp
public void ExportXml(string mapName, string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| mapName | String | Name der XML-Map, die exportiert werden muss |
| Pfad | String | Der Exportpfad |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und laden Sie die Excel-Datei
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Holen Sie die erste XmlMap aus der Arbeitsmappe
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Exportieren Sie XML-Daten mithilfe des Namens der XmlMap und des Ausgabedateipfads
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

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Exportiert XML‑Daten.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| mapName | String | Name der XML-Map, die exportiert werden muss |
| Stream | Stream | Der Export-Stream |

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe und füge einige Daten hinzu
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Name der zu exportierenden XML-Map – für Demonstrationszwecke verwenden wir einen Platzhalternamen
                string mapName = "SampleMap";

                try
                {
                    // Exportieren Sie die XML-Map in eine Datei mithilfe eines FileStream (String-, Stream-Überladung)
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

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


