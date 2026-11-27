---
title: "ExternalLinkCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLinkCollection‑metod. Lägger till en extern länk"
type: docs
url: /sv/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

Lägger till en extern länk.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Det externa filnamnet. |
| sheetNames | String[] | Alla bladnamn i den externa filen. |

### Returvärde

Positionen för det externa namnet i den här listan.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta samlingen av externa länkar
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Förbered parametrar för Add‑metoden
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Anropa Add‑metoden med parametrarna (String, String[])
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // Visa information om den tillagda externa länken
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
            
            // Spara arbetsboken
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Se även

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

Lägg till en extern länk.

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directoryType | DirectoryType | Katalogtypen för filnamnet. |
| fileName | String | filnamnet. |
| sheetNames | String[] | Alla bladnamn i den externa filen. |

### Returvärde

Positionen för det externa namnet i den här listan.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta samlingen av externa länkar
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Förbered parametrar för Add‑metoden
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Anropa Add‑metoden med parametrarna (DirectoryType, String, String[])
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // Visa information om den tillagda externa länken
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
            
            // Spara arbetsboken
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


