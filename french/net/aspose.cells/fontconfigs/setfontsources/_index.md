---
title: "FontConfigs.SetFontSources"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Définit les sources de polices"
type: docs
url: /fr/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

Définit les sources de police.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
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

    public class FontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Créer un fichier de police temporaire à des fins de démonstration
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // Créer des sources de polices
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // Appeler la méthode SetFontSources
                    FontConfigs.SetFontSources(fontSources);

                    // Vérifier que les sources de police ont été définies
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // Démontrer l'effet en vérifiant si une police est disponible
                    bool isAvailable = FontConfigs.IsFontAvailable("Arial");
                    Console.WriteLine($"Is Arial available: {isAvailable}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
                }
            }
            finally
            {
                // Nettoyer
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
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


