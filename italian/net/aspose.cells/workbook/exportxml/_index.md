---
title: "Workbook.ExportXml"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Esporta i dati XML collegati dalla mappa XML specificata"
type: docs
url: /it/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Esporta i dati XML collegati dalla mappa XML specificata.

```csharp
public void ExportXml(string mapName, string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mapName | String | nome della mappa XML da esportare |
| percorso | String | percorso di esportazione |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e carica il file Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Ottieni la prima XmlMap dalla cartella di lavoro
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Esporta i dati XML usando il nome della XmlMap e il percorso del file di output
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

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Esporta dati XML.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mapName | String | nome della mappa XML da esportare |
| stream | Stream | flusso di esportazione |

### Esempi

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
            // Crea una nuova cartella di lavoro e aggiungi alcuni dati
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Nome della mappa XML da esportare – per scopi dimostrativi utilizziamo un nome segnaposto
                string mapName = "SampleMap";

                try
                {
                    // Esporta la mappa XML in un file usando un FileStream (sovraccarico String, Stream)
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

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


