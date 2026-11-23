---
title: "Enum DirectoryType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DirectoryType enum. Représente le type de répertoire du nom de fichier"
type: docs
url: /fr/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

Représente le type de répertoire du nom de fichier.

```csharp
public enum DirectoryType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Volume | `0` | Représente une lettre de lecteur MS-DOS. Elle est suivie de la lettre du lecteur. Ou des noms de fichiers UNC, tels que \\server\share\myfile.xls |
| SameVolume | `1` | Indique que le classeur source se trouve sur le même lecteur que le classeur dépendant (la lettre du lecteur est omise) |
| DownDirectory | `2` | Indique que le classeur source se trouve dans un sous-répertoire du répertoire actuel. |
| UpDirectory | `3` | Indique que le classeur source se trouve dans le répertoire parent du répertoire actuel. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Ajouter un lien externe au classeur
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // Ajouter un lien externe avec DirectoryType.Volume
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // Récupérer le lien externe ajouté
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // Afficher les détails du lien externe
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // Enregistrez le classeur
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


