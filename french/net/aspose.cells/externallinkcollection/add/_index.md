---
title: "ExternalLinkCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ExternalLinkCollection méthode. Ajoute un lien externe"
type: docs
url: /fr/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

Ajoute un lien externe.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom de fichier externe. |
| sheetNames | String[] | Tous les noms de feuilles du fichier externe. |

### Valeur de retour

La position du nom externe dans cette liste.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez la collection de liens externes
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Préparer les paramètres pour la méthode Add
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Appeler la méthode Add avec les paramètres (String, String[])
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // Afficher les informations du lien externe ajouté
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
            
            // Enregistrez le classeur
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

Ajoutez un lien externe .

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| directoryType | DirectoryType | Le type de répertoire du nom de fichier. |
| fileName | String | le nom de fichier. |
| sheetNames | String[] | Tous les noms de feuilles du fichier externe. |

### Valeur de retour

La position du nom externe dans cette liste.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez la collection de liens externes
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Préparer les paramètres pour la méthode Add
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Appeler la méthode Add avec les paramètres (DirectoryType, String, String[])
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // Afficher les informations sur le lien externe ajouté
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
            
            // Enregistrez le classeur
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


