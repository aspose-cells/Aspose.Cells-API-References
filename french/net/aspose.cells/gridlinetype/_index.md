---
title: "Enum GridlineType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridlineType enum. Énumère les types de lignes de grille"
type: docs
url: /fr/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Énumère le type de ligne de grille.

```csharp
public enum GridlineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Dotted | `0` | Représente une ligne pointillée. |
| Hair | `1` | Représente une ligne très fine. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des options d'enregistrement et définir le type de ligne de grille
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // Ajouter des données d'exemple pour voir les lignes de grille
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // Enregistrer le classeur avec les options d'enregistrement
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


