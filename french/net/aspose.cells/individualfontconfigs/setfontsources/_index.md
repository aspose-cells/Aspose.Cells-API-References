---
title: "IndividualFontConfigs.SetFontSources"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IndividualFontConfigs. Définit les sources de police"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

Définit les sources de police.

```csharp
public void SetFontSources(FontSourceBase[] sources)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sources | FontSourceBase[] | Un tableau de sources contenant des polices TrueType. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IndividualFontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Créer des configurations de police individuelles
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Préparer les sources de police - en utilisant à la fois des sources de dossiers et des sources de police en mémoire
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // Appeler SetFontSources avec les sources de police préparées
                fontConfigs.SetFontSources(fontSources);

                Console.WriteLine("Font sources set successfully:");
                foreach (var source in fontConfigs.GetFontSources())
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                    else if (source is MemoryFontSource memorySource)
                    {
                        Console.WriteLine($"- Memory font with data length: {memorySource.FontData.Length} bytes");
                    }
                }

                // Créer un classeur pour démontrer l'effet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Utiliser une police qui devrait être disponible à partir des sources
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // Enregistrez le classeur
                workbook.Save("SetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


