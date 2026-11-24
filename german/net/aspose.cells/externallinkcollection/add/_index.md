---
title: "ExternalLinkCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLinkCollection-Methode. Fügt einen externen Link hinzu"
type: docs
url: /de/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

Fügt einen externen Link hinzu.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der externe Dateiname. |
| sheetNames | String[] | Alle Blattnamen der externen Datei. |

### Rückgabewert

Die Position des externen Namens in dieser Liste.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Holen Sie die Sammlung externer Links
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Parameter für die Add-Methode vorbereiten
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Rufen Sie die Add-Methode mit den Parametern (String, String[]) auf
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // Informationen zum hinzugefügten externen Link anzeigen
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link file: {link.DataSource}");
                Console.WriteLine("Referenced sheets:");
                foreach (string sheet in sheetNames)
                {
                    Console.WriteLine($"- {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

Fügen Sie einen externen Link hinzu.

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| directoryType | DirectoryType | Der Verzeichnistyp des Dateinamens. |
| fileName | String | der Dateiname. |
| sheetNames | String[] | Alle Blattnamen der externen Datei. |

### Rückgabewert

Die Position des externen Namens in dieser Liste.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Holen Sie die Sammlung externer Links
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Parameter für die Add-Methode vorbereiten
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Rufen Sie die Add-Methode mit den Parametern (DirectoryType, String, String[]) auf
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // Informationen über den hinzugefügten externen Link anzeigen
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link references: {link.DataSource}");
                foreach (string sheet in sheetNames) // Changed from link.SheetNames to sheetNames
                {
                    Console.WriteLine($" - References sheet: {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


