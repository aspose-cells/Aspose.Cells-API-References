---
title: "MemoryFontSource.FontData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MemoryFontSource. Données de police binaires"
type: docs
url: /fr/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

Données de police binaires.

```csharp
public byte[] FontData { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyFontDataDemo
    {
        public static void Run()
        {
            // Chargez un fichier de police TrueType en mémoire
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // Créer une instance MemoryFontSource avec les données de police
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // Afficher la valeur actuelle de FontData (les 10 premiers octets à titre de démonstration)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer les paramètres de police et ajouter notre source de police en mémoire
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Appliquer les configurations de police globalement (pas spécifiques au classeur)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Créer un style avec la police personnalisée
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // Appliquer le style à une cellule
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // Enregistrez le classeur
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


