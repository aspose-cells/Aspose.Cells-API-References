---
title: "Classe OdsSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.OdsSaveOptions. Représente les options d’enregistrement du fichier ods"
type: docs
url: /fr/net/aspose.cells/odssaveoptions/
---
## OdsSaveOptions class

Représente les options d'enregistrement du fichier ODS.

```csharp
public class OdsSaveOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OdsSaveOptions](odssaveoptions/#constructor)() | Crée les options d’enregistrement du fichier ods. |
| [OdsSaveOptions](odssaveoptions/#constructor_1)(SaveFormat) | Crée les options d’enregistrement du fichier ods. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s’il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l’enregistrement du fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n’existe pas, le répertoire sera créé automatiquement avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s’il faut chiffrer les propriétés du document lors de l’enregistrement au format .xls. La valeur par défaut est vraie.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [GeneratorType](../../aspose.cells/odssaveoptions/generatortype/) { get; set; } | Obtient et définit le générateur du fichier ods. |
| [IgnorePivotTables](../../aspose.cells/odssaveoptions/ignorepivottables/) { get; set; } | Indique s’il faut enregistrer les tableaux croisés dynamiques. |
| [IsStrictSchema11](../../aspose.cells/odssaveoptions/isstrictschema11/) { get; set; } | (**Obsolète.**) Indique si le fichier ods doit être enregistré au format ODF version 1.1. La valeur par défaut est false. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique s’il faut fusionner les zones de mise en forme conditionnelle et de validation avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [OdfStrictVersion](../../aspose.cells/odssaveoptions/odfstrictversion/) { get; set; } | Obtient et définit la version ODF. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique s’il faut mettre en cache les dernières données du graphique.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format du fichier enregistré.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique s’il faut trier les noms définis externes avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique s’il faut trier les noms définis avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique s’il faut mettre à jour le paramètre smart art. La valeur par défaut est false.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique s’il faut valider les cellules fusionnées avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../saveoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsSaveOptionsDemo
    {
        public static void OdsSaveOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Créez une instance de OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Définition des propriétés
            saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
            saveOptions.IsStrictSchema11 = true;
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Enregistrez le classeur au format ODS avec les options spécifiées
            workbook.Save("OdsSaveOptionsExample.ods", saveOptions);

            return;
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


