---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfPlaceHolders. Indique si l'index ou le nom de la feuille doit toujours être ajouté au chemin du fichier. La valeur par défaut est false, ce qui signifie que lorsqu'il n'y a qu'une seule feuille, l'index et le nom de la feuille ainsi que le préfixe correspondant prefixSheetNamePrefix ne seront pas ajoutés au chemin du fichier"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

Indique si l'index ou le nom de la feuille doit toujours être ajouté au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule feuille, l'index et le nom de la feuille ainsi que le préfixe correspondant ([`SheetNamePrefix`](../sheetnameprefix/)) ne seront pas ajoutés au chemin du fichier.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Créer un classeur avec deux feuilles pour démontrer les différences de chemin
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Configurer le fournisseur avec un espace réservé d'index de feuille
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // Démontrer le décalage d'index de feuille (facultatif)
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // Enregistrer avec l'index de feuille uniquement lorsqu'il y a plusieurs feuilles (comportement par défaut)
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // Forcer l'index de feuille dans les noms de fichiers même pour une seule feuille
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // Configurer les options d'enregistrement au format JSON pour activer le découpage
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // Configurer le fournisseur avec les options d'enregistrement
            provider.SaveOptionsTemplate = saveOptions;

            // Enregistrer avec des chemins déterminés par le fournisseur
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


