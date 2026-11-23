---
title: "IndividualFontConfigs.GetFontSources"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IndividualFontConfigs. Obtient une copie du tableau contenant la liste des sources"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

Obtient une copie du tableau contenant la liste des sources

```csharp
public FontSourceBase[] GetFontSources()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // Créer des configurations de police individuelles
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Définir certaines sources de polices (dossiers contenant des polices)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // Obtenir les sources de police actuelles
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // Créer un classeur pour démontrer l'effet
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // Utiliser les configurations de polices lors de la création de styles ou du travail avec les polices
                // (Le classeur n'a pas de propriété FontConfigs, donc nous supprimons cette ligne)
                Worksheet worksheet = workbook.Worksheets[0];

                // Utiliser une police personnalisée qui pourrait se trouver dans l'un des dossiers
                Style style = workbook.CreateStyle();
                style.Font.Name = "SomeCustomFont";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with custom font");

                Console.WriteLine("Workbook created with custom font configurations.");
                workbook.Save("MethodGetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSources method: {ex.Message}");
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


