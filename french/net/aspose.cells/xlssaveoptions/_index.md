---
title: "Classe XlsSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.XlsSaveOptions class. Représente les options d'enregistrement pour le format de fichier Excel 972003 xls et xlt"
type: docs
url: /fr/net/aspose.cells/xlssaveoptions/
---
## XlsSaveOptions class

Représente les options d'enregistrement pour le format de fichier Excel 97-2003 : xls et xlt.

```csharp
public class XlsSaveOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [XlsSaveOptions](xlssaveoptions/#constructor)() | Crée des options pour enregistrer le fichier Excel 97-2003 xls. |
| [XlsSaveOptions](xlssaveoptions/#constructor_1)(SaveFormat) | Crée des options pour enregistrer le fichier Excel 97-2003 xls/xlt. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s’il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l’enregistrement du fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n’existe pas, le répertoire sera créé automatiquement avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s’il faut chiffrer les propriétés du document lors de l’enregistrement au format .xls. La valeur par défaut est vraie.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [IsTemplate](../../aspose.cells/xlssaveoptions/istemplate/) { get; set; } | (**Obsolete.**) Indique s'il faut enregistrer un fichier modèle. |
| [LightCellsDataProvider](../../aspose.cells/xlssaveoptions/lightcellsdataprovider/) { get; set; } | Le fournisseur de données pour enregistrer le classeur en mode léger. |
| [MatchColor](../../aspose.cells/xlssaveoptions/matchcolor/) { get; set; } | Indique si la couleur de police correspond, car il y a 56 couleurs dans la palette de couleurs standard. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique s’il faut fusionner les zones de mise en forme conditionnelle et de validation avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique s’il faut mettre en cache les dernières données du graphique.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format du fichier enregistré.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique s’il faut trier les noms définis externes avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique s’il faut trier les noms définis avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique s’il faut mettre à jour le paramètre smart art. La valeur par défaut est false.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique s’il faut valider les cellules fusionnées avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/xlssaveoptions/wpscompatibility/) { get; set; } | (**Obsolete.**) Indique s'il faut rendre le xls plus compatible avec WPS. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsDemo
    {
        public static void XlsSaveOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Créer une instance de XlsSaveOptions
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Définition des propriétés
            saveOptions.MatchColor = true;
            saveOptions.ClearData = false;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Enregistrez le classeur avec les options d'enregistrement spécifiées
            workbook.Save("XlsSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


