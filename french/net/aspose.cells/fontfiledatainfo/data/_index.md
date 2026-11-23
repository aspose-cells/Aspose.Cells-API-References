---
title: "FontFileDataInfo.Data"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontFileDataInfo. Obtient les données binaires du fichier de police"
type: docs
url: /fr/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

Obtient les données binaires du fichier de police.

```csharp
public byte[] Data { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Charger un fichier de police (remplacez par le chemin réel du fichier de police)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Créer une instance de FontConfigs et ajouter la police
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // Dans une utilisation réelle, FontFileDataInfo serait obtenu à partir de la bibliothèque
            // À des fins de démonstration, nous allons simplement montrer comment vous l'utiliseriez si vous en aviez un
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // Afficher les informations sur les données de la police (si disponibles)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // Dans une utilisation réelle, la propriété Data serait utilisée pour accéder aux données binaires de la police
            // Par exemple, vous pourriez l'enregistrer dans un fichier :
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // Enregistrer le classeur (la police affecterait le rendu si elle est utilisée dans les cellules)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


