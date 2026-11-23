---
title: "Classe LowCodeSaveOptionsProviderOfAssembling"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling. Implémentation pour fournir des options d’enregistrement qui enregistrent les parties découpées dans des fichiers et dont le chemin du fichier résultant est nommé comme il peut contenir les répertoires PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

Implémentation pour fournir des options d’enregistrement qui enregistrent les parties découpées dans des fichiers et dont le chemin du fichier résultant est nommé comme (il peut contenir des répertoires) : [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(ou SheetName) +[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Indique s’il faut toujours ajouter l’index ou le nom de la feuille au chemin du fichier. La valeur par défaut est false, c’est‑à‑dire que lorsqu’il n’y a qu’une seule feuille, l’index (ou le nom) de la feuille et le préfixe correspondant ne seront pas ajoutés au chemin du fichier. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Indique s’il faut toujours ajouter l’index de la partie découpée au chemin du fichier. La valeur par défaut est false, c’est‑à‑dire que lorsqu’il n’y a qu’une seule partie découpée, l’index de la partie et le préfixe correspondant ne seront pas ajoutés au chemin du fichier. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Partie d’en‑tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin du fichier. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Partie de fin (après les numéros de séquence) du chemin du fichier. Elle doit inclure l’extension du nom de fichier. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | Le modèle pour créer une instance d’options d’enregistrement dans [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Décalage de l’index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Préfixe pour l’index de la feuille de calcul. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Décalage de l’index de la partie découpée entre celui utilisé dans le chemin du fichier et sa valeur réelle ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Préfixe pour l’index de la partie découpée. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Indique si le chemin du fichier est construit avec le nom de la feuille au lieu de l’index de la feuille. La valeur par défaut est false. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Libère les ressources après le traitement de la partie découpée actuelle (hérité de [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Obtient les options d’enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // Initialiser et configurer le fournisseur d’options d’enregistrement
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Configurer les options d’enregistrement XLSX avec découpage en utilisant LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Enregistrer le classeur avec les options activées par le fournisseur en utilisant le format d’enregistrement correct
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### Voir aussi

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


