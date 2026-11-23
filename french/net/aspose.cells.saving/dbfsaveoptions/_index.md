---
title: "Classe DbfSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Saving.DbfSaveOptions. Représente les options d'enregistrement du fichier dbf"
type: docs
url: /fr/net/aspose.cells.saving/dbfsaveoptions/
---
## DbfSaveOptions class

Représente les options d'enregistrement du fichier dbf

```csharp
public class DbfSaveOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DbfSaveOptions](dbfsaveoptions/)() | Les options d'enregistrement du fichier .dbf. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s'il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Vide le classeur après l'enregistrement du fichier (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si true et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. La valeur par défaut est true.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportAsString](../../aspose.cells.saving/dbfsaveoptions/exportasstring/) { get; set; } | Indique si l'exportation se fait sous forme de valeur chaîne |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique si les zones de mise en forme conditionnelle et de validation sont fusionnées avant l’enregistrement du fichier.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique si les dernières données du graphique doivent être mises en cache.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format de fichier d’enregistrement.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique si le tri des noms définis externes est effectué avant l'enregistrement du fichier.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique si le tri des noms définis est effectué avant l'enregistrement du fichier.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique si la mise à jour du paramètre SmartArt est activée. La valeur par défaut est false.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique si la validation des cellules fusionnées est effectuée avant d'enregistrer le fichier.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassDbfSaveOptionsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer une instance de DbfSaveOptions
            DbfSaveOptions saveOptions = new DbfSaveOptions();
            
            // Définir la propriété ExportAsString
            saveOptions.ExportAsString = true;

            // Enregistrer le classeur avec les options d'enregistrement DBF
            workbook.Save("output.dbf", saveOptions);

            Console.WriteLine("Workbook saved as DBF with ExportAsString set to true.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


