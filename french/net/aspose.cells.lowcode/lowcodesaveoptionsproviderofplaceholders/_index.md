---
title: "Classe LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders. Implémentation pour fournir des options d’enregistrement qui enregistrent les parties découpées dans des fichiers et dont le chemin du fichier résultant est défini avec des espaces réservés"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

Implémentation pour fournir des options d'enregistrement qui enregistrent les parties découpées dans des fichiers et le chemin du fichier résultant est défini avec des espaces réservés.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Instancie une instance pour fournir des options d’enregistrement selon les modèles spécifiés. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Indique s’il faut toujours ajouter l’index ou le nom de la feuille au chemin du fichier. La valeur par défaut est false, c’est‑à‑dire que lorsqu’il n’y a qu’une seule feuille, l’index et le nom de la feuille ainsi que le préfixe correspondant ([`SheetNamePrefix`](./sheetnameprefix/)) ne seront pas ajoutés au chemin du fichier. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Indique s’il faut toujours ajouter l’index de la partie découpée au chemin du fichier. La valeur par défaut est false, c’est‑à‑dire que lorsqu’il n’y a qu’une seule partie découpée, l’index de la partie découpée et le préfixe correspondant ([`SplitPartPrefix`](./splitpartprefix/)) ne seront pas ajoutés au chemin du fichier. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | Le modèle pour créer une instance d’options d’enregistrement dans [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Décalage de l’index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Préfixe pour l’index de la feuille de calcul. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Préfixe pour l’index de la feuille de calcul. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Décalage de l’index de la partie découpée entre celui utilisé dans le chemin du fichier et sa valeur réelle ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Préfixe pour l’index de la partie découpée. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Libère les ressources après le traitement de la partie découpée actuelle (hérité de [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Obtient les options d’enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir la feuille de calcul avec des données d'exemple
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Créer un fournisseur avec un modèle de chemin contenant des espaces réservés
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // Configurer les propriétés du fournisseur
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // Configurer le modèle d’options d’enregistrement
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Configurer les options d’image ou d’impression pour le rendu découpé
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // Créer un rendu de feuille avec la configuration de découpage
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### Voir aussi

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


