---
title: "Énumération SaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.SaveFormat enum. Représente le format dans lequel le classeur est enregistré"
type: docs
url: /fr/net/aspose.cells/saveformat/
---
## SaveFormat enumeration

Représente le format dans lequel le classeur est enregistré.

```csharp
public enum SaveFormat
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Csv | `1` | Fichier texte Valeurs séparées par des virgules (CSV). |
| CSV | `1` | Fichier texte Valeurs séparées par des virgules (CSV). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Csv. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Xlsx | `6` | Représente un fichier xlsx. |
| Xlsm | `7` | Représente un fichier xlsm qui active les macros. |
| Xltx | `8` | Représente un fichier xltx. |
| Xltm | `9` | Représente un fichier xltm qui active les macros. |
| Xlam | `10` | Représente un fichier xltm qui active les macros d'add-in. |
| Tsv | `11` | Fichier texte Valeurs séparées par des tabulations (TSV). |
| TSV | `11` | Fichier texte Valeurs séparées par des tabulations (TSV). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Tsv. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| TabDelimited | `11` | Représente un fichier texte à délimitation par tabulation, identique à Tsv. |
| Html | `12` | Représente un fichier html. |
| MHtml | `17` | Représente un fichier mhtml. |
| Ods | `14` | Fichier Open Document Sheet (ODS). |
| ODS | `14` | Fichier Open Document Sheet (ODS). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Ods. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Excel97To2003 | `5` | Représente un fichier Excel97-2003 xls. |
| SpreadsheetML | `15` | Représente un fichier Excel 2003 xml. |
| Xlsb | `16` | Représente un fichier xlsb. |
| Auto | `0` | Si le fichier est enregistré sur le disque, le format du fichier correspond à l'extension du nom de fichier. Si le fichier est enregistré dans le flux, le format du fichier est xlsx. |
| Unknown | `255` | Représente un format non reconnu, ne peut pas être enregistré. |
| Pdf | `13` | Représente un fichier PDF. |
| Xps | `20` | Format XPS (XML Paper Specification). |
| XPS | `20` | Format XPS (XML Paper Specification). NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Xps. Cette propriété sera supprimée 6 mois plus tard depuis avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Tiff | `21` | Représente un fichier TIFF. |
| TIFF | `21` | Représente un fichier TIFF. NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Tiff. Cette propriété sera supprimée 6 mois plus tard depuis avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Svg | `28` | Fichier SVG. |
| SVG | `28` | Fichier SVG. NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Svg. Cette propriété sera supprimée 6 mois plus tard depuis avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Dif | `30` | Format d'échange de données. |
| Ots | `31` | Fichier Open Document Template Sheet (OTS). |
| Xlt | `32` | Fichier modèle Excel 97-2003. |
| Xml | `51` | Représente un fichier xml simple. |
| Numbers | `56` | Représente un fichier Numbers depuis 2014 de Apple Inc. |
| Markdown | `57` | Représente un document markdown. |
| Fods | `59` | Représente le format de fichier OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | Représente le format de fichier OpenDocument Flat XML Spreadsheet (.fods). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Fods. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Sxc | `60` | Représente le format de fichier StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | Représente le format de fichier StarOffice Calc Spreadsheet (.sxc). NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Sxc. Cette propriété sera supprimée 6 mois après avril 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Pptx | `61` | Représente un fichier .pptx. |
| Docx | `62` | Représente un fichier .docx. |
| Emf | `258` | Metafile Windows amélioré. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Bmp | `263` | Bitmap Windows |
| Gif | `322` | Gif |
| Json | `513` | Json |
| SqlScript | `514` | SQL |
| XHtml | `771` | Représente un fichier XHtml. Veuillez utiliser la propriété [`HtmlVersion`](../htmlsaveoptions/htmlversion/). Cette propriété sera supprimée dans 6 mois à partir de mars 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer. |
| Epub | `772` | Représente un fichier Epub. |
| Azw3 | `773` | Représente un fichier Azw3. |
| Pcl | `1025` | PCL (Langage de commande d'imprimante) |
| Ofd | `1026` | OFD (Document à mise en page fixe) |
| Dbf | `515` | Fichier de données Xbase |

### Exemples

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class SaveFormatDemo
    {
        public static void SaveFormatExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Enregistrez le classeur dans différents formats
            workbook.Save("SaveFormatExample.xlsx", SaveFormat.Xlsx);
            workbook.Save("SaveFormatExample.xls", SaveFormat.Excel97To2003);
            workbook.Save("SaveFormatExample.csv", SaveFormat.Csv);
            workbook.Save("SaveFormatExample.pdf", SaveFormat.Pdf);
            workbook.Save("SaveFormatExample.html", SaveFormat.Html);

            // Afficher les résultats
            Console.WriteLine("Workbook saved in multiple formats.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


