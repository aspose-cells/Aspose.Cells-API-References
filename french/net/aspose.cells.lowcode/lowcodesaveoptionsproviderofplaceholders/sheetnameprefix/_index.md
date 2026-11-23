---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfPlaceHolders. Préfixe pour l'index de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

Préfixe pour l’index de la feuille de calcul.

```csharp
public string SheetNamePrefix { get; set; }
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

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // Initialiser le fournisseur avec un modèle de chemin contenant le placeholder de feuille
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Afficher la valeur initiale de SheetNamePrefix (vide par défaut)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // Définir un nouveau préfixe et garantir que la génération du chemin inclut les informations de feuille
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // Configurer les options d'enregistrement avec le format correct
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // Enregistrer le classeur en utilisant le fournisseur - génère "output_Q4_SalesData.xlsx" et "output_Q4_FinancialReport.xlsx"
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


