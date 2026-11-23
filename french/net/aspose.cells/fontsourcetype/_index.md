---
title: "Énumération FontSourceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.FontSourceType enum. Spécifie le type d’une source de police"
type: docs
url: /fr/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Spécifie le type d'une source de police.

```csharp
public enum FontSourceType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| FontFile | `0` | représente un fichier de police unique. |
| FontsFolder | `1` | Représente un dossier contenant des fichiers de police. |
| MemoryFont | `2` | Représente une police unique en mémoire. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontrez les valeurs de l’enum FontSourceType
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Créez les paramètres de police et utilisez FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Appliquez la police à une cellule
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Enregistrer le résultat
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


