---
title: "Énumération FileFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.FileFormatType. Représente les types de formats de fichier"
type: docs
url: /fr/net/aspose.cells/fileformattype/
---
## FileFormatType enumeration

Représente les types de format de fichier.

```csharp
public enum FileFormatType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Csv | `1` | Fichier texte Valeurs séparées par des virgules (CSV). |
| Xlsx | `6` | Fichier Office Open XML SpreadsheetML (sans macro). |
| Xlsm | `7` | Fichier Office Open XML SpreadsheetML (avec macro). |
| Xltx | `8` | Modèle Office Open XML SpreadsheetML (sans macro). |
| Xltm | `9` | Modèle Office Open XML SpreadsheetML (avec macro). |
| Xlam | `10` | Fichier Office Open XML SpreadsheetML addin (avec macro). |
| Tsv | `11` | Fichier texte Valeurs séparées par des tabulations (TSV). |
| TabDelimited | `11` | Fichier texte Tab-Separated Values (TSV), identique à Tsv. |
| Html | `12` | Format HTML. |
| MHtml | `17` | Format MHTML (archive Web). |
| Ods | `14` | Fichier Open Document Sheet (ODS). |
| Excel97To2003 | `5` | Fichier feuille de calcul Excel97-2003. |
| SpreadsheetML | `15` | Fichier de données XML Excel 2003. |
| Xlsb | `16` | Le format de fichier binaire Excel (.xlsb) |
| Unknown | `255` | Représente un format non reconnu, ne peut pas être chargé. |
| Pdf | `13` | Format PDF (Adobe Portable Document). |
| Xps | `20` | Format XPS (XML Paper Specification). |
| Tiff | `21` | Représente un fichier TIFF. |
| Svg | `28` | Fichier SVG. |
| Excel95 | `22` | Représente un fichier Excel95 xls. |
| Excel4 | `23` | Représente un fichier Excel4.0 xls. |
| Excel3 | `24` | Représente un fichier Excel3.0 xls. |
| Excel2 | `25` | Représente un fichier Excel2.1 xls. |
| Pptx | `26` | Représente un fichier pptx. |
| Docx | `27` | Représente un fichier docx. |
| Dif | `30` | Format d'échange de données. |
| Doc | `31` | Représente un fichier doc. |
| Ppt | `32` | Représente un fichier ppt. |
| MapiMessage | `33` | Représente un fichier email. |
| MsEquation | `34` | Représente l'objet MS Equation 3.0. |
| Ole10Native | `35` | Représente l'objet natif intégré. |
| Vsd | `36` | Représente le format binaire MS Visio VSD. |
| Vsdx | `37` | Représente le format de fichier MS Visio 2013 VSDX. |
| Docm | `38` | Représente un fichier docm. |
| Dotx | `39` | Représente un fichier dotx. |
| Dotm | `40` | Représente un fichier dotm. |
| Pptm | `41` | Représente un fichier pptm. |
| Potx | `42` | Représente un fichier Potx. |
| Potm | `43` | Représente un fichier Potm. |
| Ppsx | `44` | Représente un fichier ppsx. |
| Ppsm | `45` | Représente un fichier ppsm. |
| Ooxml | `46` | Représente un fichier Office Open XML (tel que xlsx, docx, pptx, etc). |
| Odt | `47` | Représente un fichier ODT. |
| Odp | `48` | Représente un fichier ODP. |
| Odf | `49` | Représente un fichier ODF. |
| Odg | `50` | Représente un fichier ODG. |
| Xml | `51` | Représente un fichier xml simple. |
| Xlt | `52` | Modèle de feuille de calcul Excel97-2003. |
| Ott | `53` | Représente un fichier OTT. |
| Bmp | `54` | Représente un fichier BMP. |
| Ots | `55` | Représente un fichier ots. |
| Numbers | `56` | Représente le format de fichier Numbers 9.0 d'Apple Inc. |
| Numbers09 | `56` | Représente le format de fichier Numbers 9.0 d'Apple Inc. |
| Markdown | `57` | Représente un document markdown. |
| GraphChart | `58` | Représente un graphique intégré. |
| Fods | `59` | Représente le format de fichier OpenDocument Flat XML Spreadsheet (.fods). |
| Sxc | `60` | Représente le format de fichier StarOffice Calc Spreadsheet (.sxc). |
| Otp | `61` | Représente un fichier OTP. |
| Numbers35 | `62` | Représente le format de fichier Numbers 3.5 depuis 2014 d'Apple Inc. |
| Ole | `64` | Représente l'objet OLE intégré. |
| Emf | `258` | Metafile Windows amélioré. |
| Wmf | `259` | Metafile Windows. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Gif | `322` | Gif |
| WebP | `323` | Webp |
| Json | `513` | Json |
| SqlScript | `514` | SQL |
| Dbf | `515` | Fichier de données Xbase |
| FlatOpc | `516` | Fichier opc plat |
| XHtml | `771` | Représente le fichier XHtml. |
| OneNote | `772` | Représente le fichier One Note. |
| MicrosoftCabinet | `773` | Représente le fichier Microsoft Cabinet. |
| Rtf | `774` | Rtf |
| Epub | `775` | EPUB |
| Azw3 | `777` | AZW3 |
| Chm | `784` | CHM |
| Oxps | `776` | OXPS (Open XML Paper Specification) format. |
| GZip | `35615` | Représente le fichier GZip. |
| Otg | `1025` | Représente un fichier OTG. |
| Odb | `1026` | Représente un fichier Odb. |
| Ofd | `1029` | Représente un fichier Ofd. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatTypeDemo
    {
        public static void FileFormatTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir le nom de la feuille de calcul
            worksheet.Name = "File Format Example";

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("File Format Type");
            worksheet.Cells["A2"].PutValue(FileFormatType.Csv);
            worksheet.Cells["A3"].PutValue(FileFormatType.Xlsx);
            worksheet.Cells["A4"].PutValue(FileFormatType.Pdf);
            worksheet.Cells["A5"].PutValue(FileFormatType.Xlsm);

            // Afficher les types de format de fichier
            for (int i = 2; i <= 5; i++)
            {
                var fileFormat = worksheet.Cells[$"A{i}"].StringValue;
                Console.WriteLine($"Row {i}: {fileFormat}");
            }

            // Enregistrez le classeur
            workbook.Save("FileFormatTypeExample.xlsx");
            workbook.Save("FileFormatTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


