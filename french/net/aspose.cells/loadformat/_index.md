---
title: "Enum LoadFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.LoadFormat. Représente le format de fichier à charger."
type: docs
url: /fr/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

Représente le format de fichier de chargement.

```csharp
public enum LoadFormat
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Auto | `0` | Représente la reconnaissance automatique du format. |
| Csv | `1` | Fichier texte Valeurs séparées par des virgules (CSV). |
| CSV | `1` | Fichier texte Valeurs séparées par des virgules (CSV). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Csv. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Xlsx | `6` | Représente un classeur ou modèle Office Open XML spreadsheetML, avec ou sans macros. |
| Tsv | `11` | Fichier texte Valeurs séparées par des tabulations (TSV). |
| TSV | `11` | Fichier texte Valeurs séparées par des tabulations (TSV). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Tsv. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| TabDelimited | `11` | Représente un fichier texte à délimitation par tabulation, identique à Tsv. |
| Html | `12` | Représente un fichier html. |
| MHtml | `13` | Représente un fichier mhtml. |
| Ods | `14` | Fichier Open Document Sheet (ODS). |
| ODS | `14` | Fichier Open Document Sheet (ODS). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Ods. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Excel97To2003 | `5` | Représente un fichier Excel97-2003 xls. |
| SpreadsheetML | `15` | Représente un fichier Excel 2003 xml. |
| Xlsb | `16` | Représente un fichier xlsb. |
| Ots | `31` | Fichier Open Document Template Sheet (OTS). |
| Numbers | `56` | Représente un fichier Numbers. |
| Fods | `59` | Représente le format de fichier OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | Représente le format de fichier OpenDocument Flat XML Spreadsheet (.fods). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Fods. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Sxc | `60` | Représente le format de fichier StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | Représente le format de fichier StarOffice Calc Spreadsheet (.sxc). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Sxc. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Xml | `51` | Représente un fichier xml simple. |
| Epub | `52` | Représente un fichier EPUB. |
| Azw3 | `53` | Représente un fichier AZW3. |
| Chm | `54` | Représente un fichier CHM. |
| Markdown | `55` | Représente un fichier Markdown. |
| Unknown | `255` | Représente un format non reconnu, ne peut pas être chargé. |
| Image | `254` | Image |
| Json | `513` | Json |
| Dif | `30` | Format d'échange de données. |
| Dbf | `515` | Fichier de données Xbase |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // Chargez un fichier Excel dans différents formats en utilisant Aspose.Cells
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // Déterminez le format de chargement en fonction de l'extension du fichier
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // Créez LoadOptions avec le LoadFormat déterminé
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // Chargez le classeur avec les options de chargement spécifiées
                Workbook workbook = new Workbook(filePath, loadOptions);

                // Effectuez quelques opérations sur le classeur
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // Enregistrez le classeur dans un nouveau fichier
                string outputFilePath = $"output_{System.IO.Path.GetFileName(filePath)}";
                workbook.Save(outputFilePath);
                Console.WriteLine($"Saved file as: {outputFilePath}");
            }
        }

        private static LoadFormat GetLoadFormat(string filePath)
        {
            string extension = System.IO.Path.GetExtension(filePath).ToLower();
            switch (extension)
            {
                case ".xlsx":
                    return LoadFormat.Xlsx;
                case ".xls":
                    return LoadFormat.Excel97To2003;
                case ".csv":
                    return LoadFormat.Csv;
                case ".json":
                    return LoadFormat.Json;
                default:
                    return LoadFormat.Auto;
            }
        }
    }

}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


