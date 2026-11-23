---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfPlaceHolders. Préfixe pour l'index de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

Préfixe pour l’index de la feuille de calcul.

```csharp
public string SheetIndexPrefix { get; set; }
```

### Remarques

S'il n'y a qu'une seule feuille de calcul et que [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) est faux, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin de fichier résultant.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec plusieurs feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Créer une instance de LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Afficher et modifier SheetIndexPrefix
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // Définissez les autres propriétés requises
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // Démontrer l'effet de SheetIndexPrefix sur les chemins de fichier
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // Puisque nous ne pouvons pas créer et remplir SplitPartInfo directement,
                // nous allons simplement démontrer le modèle de nommage sans cela
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // Enregistrer le classeur pour démontrer le modèle de nommage
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


