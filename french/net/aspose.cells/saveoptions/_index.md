---
title: "Classe SaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.SaveOptions. Représente toutes les options d'enregistrement"
type: docs
url: /fr/net/aspose.cells/saveoptions/
---
## SaveOptions class

Représente toutes les options d'enregistrement

```csharp
public class SaveOptions
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s'il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l'enregistrement du fichier. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant l'enregistrement du fichier. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. La valeur par défaut est vraie. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant l'enregistrement du fichier. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique s'il faut mettre en cache les dernières données du graphique. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format du fichier d'enregistrement. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique si le tri des noms définis externes doit être effectué avant d'enregistrer le fichier. |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique si le tri des noms définis doit être effectué avant d'enregistrer le fichier. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique si la mise à jour du paramètre SmartArt est activée. La valeur par défaut est false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique si la validation des cellules fusionnées doit être effectuée avant d'enregistrer le fichier. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSaveOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Créer des options d'enregistrement - enregistrer en CSV
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = ',';
            
            // Créer des options de chargement pour CSV
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);

            // Réenregistrez le classeur en utilisant les options
            Workbook resavedWorkbook = Cells_Type_SaveOptions(workbook, saveOptions, loadOptions);

            // Enregistrez le résultat dans un fichier
            resavedWorkbook.Save("output.csv", SaveFormat.Csv);
        }

        public static Workbook Cells_Type_SaveOptions(Workbook wb, SaveOptions optsSave, LoadOptions optsLoad)
        {
            using (MemoryStream ms = new MemoryStream(1048576))
            {
                wb.Save(ms, optsSave);
                ms.Position = 0;
                return new Workbook(ms, optsLoad);
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


