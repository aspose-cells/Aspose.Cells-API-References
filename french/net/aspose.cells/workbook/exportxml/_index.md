---
title: "Workbook.ExportXml"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Exporte les données XML liées par la carte XML spécifiée"
type: docs
url: /fr/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Exporte les données XML liées par la carte XML spécifiée.

```csharp
public void ExportXml(string mapName, string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mapName | String | nom de la carte XML qui doit être exportée |
| chemin | String | le chemin d'exportation |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un classeur et charger le fichier Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Obtenir le premier XmlMap du classeur
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Exporter les données XML en utilisant le nom du XmlMap et le chemin du fichier de sortie
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

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Exporte les données XML.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mapName | String | nom de la carte XML qui doit être exportée |
| stream | Stream | le flux d'exportation |

### Exemples

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
            // Créer un nouveau classeur et ajouter des données
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Nom de la carte XML à exporter – à des fins de démonstration, nous utilisons un nom de substitution
                string mapName = "SampleMap";

                try
                {
                    // Exporter la carte XML vers un fichier en utilisant un FileStream (surcharge String, Stream)
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

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


