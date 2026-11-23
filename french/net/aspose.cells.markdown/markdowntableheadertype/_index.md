---
title: "Énumération MarkdownTableHeaderType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Markdown.MarkdownTableHeaderType. Représente le type d'en-tête du tableau dans le fichier markdown"
type: docs
url: /fr/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Représente le type d'en-tête du tableau dans le fichier markdown.

```csharp
public enum MarkdownTableHeaderType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| FirstRow | `0` | Première ligne comme en-tête du tableau. |
| ColumnHeader | `1` | Nom de colonne (tel que A,B,C...) comme en-tête du tableau. |
| Empty | `2` | Une ligne d'en-tête vide. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Définir les options d'enregistrement Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Enregistrer sous fichier Markdown
            workbook.Save("output.md", saveOptions);
            
            // Vérifier la sortie
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


