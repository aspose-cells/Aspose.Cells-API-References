---
title: "Enum OoxmlCompressionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.OoxmlCompressionType enum. Le type de compression Ooxml"
type: docs
url: /fr/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

Le type de compression Ooxml

```csharp
public enum OoxmlCompressionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Level1 | `1` | La compression la plus rapide mais la moins efficace. |
| Level2 | `2` | Un peu plus lente, mais meilleure, que le niveau 1. |
| Level3 | `3` | Un peu plus lente, mais meilleure, que le niveau 2. |
| Level4 | `4` | Un peu plus lente, mais meilleure, que le niveau 3. |
| Level5 | `5` | Un peu plus lente que le niveau 4, mais avec une meilleure compression. |
| Level6 | `6` | Un bon équilibre entre vitesse et efficacité de compression. |
| Level7 | `7` | Compression plutôt bonne ! |
| Level8 | `8` | Meilleure compression que Level7 ! |
| Level9 | `9` | La "meilleure" compression, où meilleure signifie la plus grande réduction de la taille du flux de données d'entrée. C'est également la compression la plus lente. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Créer OoxmlSaveOptions et définir le type de compression
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Enregistrer le classeur avec le type de compression spécifié
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


