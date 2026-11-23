---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfPlaceHolders. Indique si l'index de la partie découpée doit toujours être ajouté au chemin du fichier. La valeur par défaut est false, ce qui signifie que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant prefixSplitPartPrefix ne seront pas ajoutés au chemin du fichier"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

Indique si l'index de la partie découpée doit toujours être ajouté au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant ([`SplitPartPrefix`](../splitpartprefix/)) ne seront pas ajoutés au chemin du fichier.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données qui ne seront pas découpées en plusieurs parties
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // Créer un fournisseur avec un modèle de chemin et une condition de découpage qui aboutit à une seule partie
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // Démontrer l'état false de la propriété (par défaut)
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // Cela générerait Result.xlsx lorsqu'il n'existe qu'une seule partie
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // Basculer la propriété et démontrer l'état true
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // Cela générerait Result_0.xlsx même avec une seule partie
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // Dans une utilisation réelle, remplacer par une opération d'enregistrement basée sur le fournisseur
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


