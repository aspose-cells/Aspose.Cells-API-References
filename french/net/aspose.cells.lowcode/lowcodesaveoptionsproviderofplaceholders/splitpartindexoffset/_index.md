---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfPlaceHolders. Décalage de l'index des parties découpées entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle valuePartIndex"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset property

Décalage de l'index de la partie fractionnée entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle ([`PartIndex`](../../splitpartinfo/partindex/)).

```csharp
public int SplitPartIndexOffset { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Créer un modèle d'options d'enregistrement low code
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();
            saveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Initialiser le fournisseur avec un modèle de chemin
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/SplitPart_{0}.xlsx");
            provider.SaveOptionsTemplate = saveOptionsTemplate;

            // Afficher et modifier SplitPartIndexOffset
            Console.WriteLine("Initial SplitPartIndexOffset: " + provider.SplitPartIndexOffset);
            provider.SplitPartIndexOffset = 1;

            // Enregistrer le classeur pour générer des parties découpées avec un index ajusté
            workbook.Save("SplitPartIndexOffsetDemo", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Generated split parts with offset applied.");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


