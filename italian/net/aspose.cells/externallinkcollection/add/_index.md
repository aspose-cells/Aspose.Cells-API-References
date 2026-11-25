---
title: "ExternalLinkCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ExternalLinkCollection. Aggiunge un collegamento esterno"
type: docs
url: /it/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

Aggiunge un collegamento esterno.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome del file esterno. |
| sheetNames | String[] | Tutti i nomi dei fogli del file esterno. |

### Valore di ritorno

La posizione del nome esterno in questo elenco.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni la raccolta di collegamenti esterni
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Prepara i parametri per il metodo Add
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Chiama il metodo Add con i parametri (String, String[])
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // Visualizza le informazioni del collegamento esterno aggiunto
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
            
            // Salva la cartella di lavoro
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

Aggiungi un collegamento esterno.

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directoryType | DirectoryType | Il tipo di directory del nome file. |
| fileName | String | il nome file. |
| sheetNames | String[] | Tutti i nomi dei fogli del file esterno. |

### Valore di ritorno

La posizione del nome esterno in questo elenco.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni la raccolta di collegamenti esterni
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Prepara i parametri per il metodo Add
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Chiama il metodo Add con i parametri (DirectoryType, String, String[])
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // Visualizza le informazioni sul collegamento esterno aggiunto
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
            
            // Salva la cartella di lavoro
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


