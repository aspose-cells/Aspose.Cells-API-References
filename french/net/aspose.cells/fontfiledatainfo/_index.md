---
title: "Classe FontFileDataInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FontFileDataInfo. Représente les informations de données du fichier de police"
type: docs
url: /fr/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Représente les informations de données du fichier de police.

```csharp
public class FontFileDataInfo
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Obtient les données binaires du fichier de police. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Obtient le type de format de police du fichier de police. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exemple : Chargement des données du fichier de police
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Remarque : FontFileDataInfo ne peut pas être instancié directement car il n'a pas de constructeur public
            // et ses propriétés sont en lecture seule. Dans un scénario réel, vous obtiendriez une instance
            // à partir d'une autre méthode API (comme FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Démontrez comment les propriétés seraient utilisées si nous avions une instance
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Démontrez l'intégration avec Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Enregistrez le classeur
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


