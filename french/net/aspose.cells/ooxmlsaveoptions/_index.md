---
title: "Class OoxmlSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.OoxmlSaveOptions. Représente les options d'enregistrement du fichier Office Open XML"
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class

Représente les options d'enregistrement du fichier Office Open XML.

```csharp
public class OoxmlSaveOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor)() | Crée les options pour enregistrer le fichier Office Open XML. |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor_1)(SaveFormat) | Crée les options pour enregistrer le fichier Office Open XML. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AsFlatOpc](../../aspose.cells/ooxmlsaveoptions/asflatopc/) { get; set; } | Indique s'il faut enregistrer en tant que fichier OPC plat pouvant être généré par le SDK Open XML. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s’il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l’enregistrement du fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CompressionType](../../aspose.cells/ooxmlsaveoptions/compressiontype/) { get; set; } | Obtient et définit le type de compression pour le fichier ooxml. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n’existe pas, le répertoire sera créé automatiquement avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [EmbedOoxmlAsOleObject](../../aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/) { get; set; } | Indique s'il faut incorporer les fichiers Ooxml d'OleObject en tant qu'objet ole. |
| [EnableZip64](../../aspose.cells/ooxmlsaveoptions/enablezip64/) { get; set; } | Utiliser les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s’il faut chiffrer les propriétés du document lors de l’enregistrement au format .xls. La valeur par défaut est vraie.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ExportCellName](../../aspose.cells/ooxmlsaveoptions/exportcellname/) { get; set; } | Indique si le nom de la cellule doit être exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si le fichier de sortie peut être accédé par SQL Server DTS, cette valeur doit être true. Mettre la valeur à false augmentera considérablement les performances et réduira la taille du fichier lors de la création de gros fichiers. La valeur par défaut est true. |
| [LightCellsDataProvider](../../aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/) { get; set; } | Le fournisseur de données pour enregistrer le classeur en mode léger. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique s’il faut fusionner les zones de mise en forme conditionnelle et de validation avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique s’il faut mettre en cache les dernières données du graphique.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format du fichier enregistré.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique s’il faut trier les noms définis externes avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique s’il faut trier les noms définis avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique s’il faut mettre à jour le paramètre smart art. La valeur par défaut est false.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [UpdateZoom](../../aspose.cells/ooxmlsaveoptions/updatezoom/) { get; set; } | Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent la mise à l'échelle de la feuille de calcul. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique s’il faut valider les cellules fusionnées avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/ooxmlsaveoptions/wpscompatibility/) { get; set; } | (**Obsolete.**) Indique s'il faut rendre le xls plus compatible avec WPS. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsDemo
    {
        public static void OoxmlSaveOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Créer une instance de OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

            // Définition des propriétés
            saveOptions.ExportCellName = true;
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = false;
            saveOptions.EmbedOoxmlAsOleObject = false;
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Enregistrer le classeur avec les options spécifiées
            workbook.Save("OoxmlSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


