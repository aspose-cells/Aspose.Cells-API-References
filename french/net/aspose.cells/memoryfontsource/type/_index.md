---
title: "MemoryFontSource.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MemoryFontSource. Retourne le type de la source de police"
type: docs
url: /fr/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

Renvoie le type de la source de police.

```csharp
public override FontSourceType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            // Chargez un fichier de police TrueType en mémoire
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Créer une instance MemoryFontSource avec les données de police
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Afficher la valeur actuelle de Type
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les sources de police en utilisant FontConfigs
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Vérifier que le type de la source de police est MemoryFont
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // Utiliser la police dans une cellule
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // Ajouter des informations sur le type de la source de police
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // Enregistrez le classeur
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


