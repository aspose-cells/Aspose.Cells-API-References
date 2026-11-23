---
title: "Classe TxtSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.TxtSaveOptions. Représente les options d'enregistrement pour le format texte csv/à séparateur de tabulation/autre."
type: docs
url: /fr/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

Représente les options d'enregistrement pour le format csv/tab délimité/autre texte.

```csharp
public class TxtSaveOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions/#constructor)() | Crée les options d'enregistrement du fichier texte. |
| [TxtSaveOptions](txtsaveoptions/#constructor_1)(SaveFormat) | Crée les options d'enregistrement du fichier texte. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AlwaysQuoted](../../aspose.cells/txtsaveoptions/alwaysquoted/) { get; set; } | (**Obsolète.**) Indique si l'ajout du caractère '"' pour chaque champ est toujours effectué. Si vrai, toutes les valeurs seront entre guillemets ; si faux, les valeurs ne seront entre guillemets que lorsque cela est nécessaire (par exemple, lorsque les valeurs contiennent des caractères spéciaux tels que '"', '\\n' ou le caractère séparateur). La valeur par défaut est false. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s’il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l’enregistrement du fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n’existe pas, le répertoire sera créé automatiquement avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding/) { get; set; } | Obtient et définit l'encodage par défaut. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s’il faut chiffrer les propriétés du document lors de l’enregistrement au format .xls. La valeur par défaut est vraie.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets/) { get; set; } | Indique si toutes les feuilles sont exportées vers le fichier texte. Si false, seule la feuille active est exportée, comme dans MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea/) { get; set; } | La plage de cellules à exporter. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix/) { get; set; } | Indique si le signe d'apostrophe doit être exporté comme partie de la valeur d'une cellule lorsque [`QuotePrefix`](../style/quoteprefix/) est vrai pour celle‑ci. La valeur par défaut est false. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy/) { get; set; } | Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow/) { get; set; } | Indique si des séparateurs doivent être générés pour une ligne vide. La valeur par défaut est false, ainsi le contenu d'une ligne vide sera vide. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider/) { get; set; } | Le fournisseur de données pour enregistrer le classeur en mode léger. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique s’il faut fusionner les zones de mise en forme conditionnelle et de validation avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype/) { get; set; } | Obtient ou définit la façon de citer les valeurs dans le fichier texte exporté. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique s’il faut mettre en cache les dernières données du graphique.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format du fichier enregistré.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [Separator](../../aspose.cells/txtsaveoptions/separator/) { get; set; } | Obtient et définit le caractère délimiteur du fichier texte. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring/) { get; set; } | Obtient et définit une valeur chaîne comme séparateur. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique s’il faut trier les noms définis externes avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique s’il faut trier les noms définis avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/) { get; set; } | Indique si les lignes et colonnes vides en début doivent être supprimées comme le fait ms excel. La valeur par défaut est true. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells/) { get; set; } | Indique si les cellules vides en fin de ligne doivent être supprimées. La valeur par défaut est false. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique s’il faut mettre à jour le paramètre smart art. La valeur par défaut est false.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique s’il faut valider les cellules fusionnées avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../saveoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtSaveOptionsDemo
    {
        public static void TxtSaveOptionsExample()
        {
            // Créer un classeur avec quelques données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Smith");
            worksheet.Cells["B3"].PutValue(25);

            // Créer un objet TxtSaveOptions et définir les propriétés
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                SeparatorString = ",",
                Encoding = Encoding.UTF8,
                AlwaysQuoted = false,
                QuoteType = TxtValueQuoteType.Normal,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                TrimLeadingBlankRowAndColumn = true,
                TrimTailingBlankCells = false,
                KeepSeparatorsForBlankRow = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                ExportQuotePrefix = false,
                ExportAllSheets = false,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Enregistrez le classeur en tant que fichier texte avec les options spécifiées
            workbook.Save("TxtSaveOptionsExample.txt", saveOptions);

            Console.WriteLine("Workbook saved successfully with TxtSaveOptions.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


