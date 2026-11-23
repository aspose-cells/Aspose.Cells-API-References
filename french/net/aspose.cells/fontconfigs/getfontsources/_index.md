---
title: "FontConfigs.GetFontSources"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Obtient une copie du tableau qui contient la liste des sources"
type: docs
url: /fr/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

Obtient une copie du tableau contenant la liste des sources

```csharp
public static FontSourceBase[] GetFontSources()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            try
            {
                // Obtenir les sources de police actuelles
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // Afficher les informations sur chaque source de police
                if (fontSources != null)
                {
                    Console.WriteLine("Current font sources:");
                    foreach (var source in fontSources)
                    {
                        Console.WriteLine($"Type: {source.GetType().Name}");
                        if (source is FolderFontSource folderSource)
                        {
                            Console.WriteLine($"Folder path: {folderSource.FolderPath}");
                            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
                        }
                        else if (source is FileFontSource fileSource)
                        {
                            Console.WriteLine($"File path: {fileSource.FilePath}");
                        }
                        else if (source is MemoryFontSource memorySource)
                        {
                            Console.WriteLine($"Font data present: {memorySource.FontData != null}");
                        }
                        Console.WriteLine();
                    }
                }
                else
                {
                    Console.WriteLine("No font sources are currently set.");
                }

                // Créer un nouveau classeur pour démontrer l'effet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Définir du texte avec une police qui pourrait utiliser ces sources
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // Enregistrez le classeur
                workbook.Save("FontConfigsGetFontSourcesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with font sources: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


