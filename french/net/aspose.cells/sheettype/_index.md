---
title: "Énumération SheetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.SheetType enum. Spécifie le type de feuille de calcul"
type: docs
url: /fr/net/aspose.cells/sheettype/
---
## SheetType enumeration

Spécifie le type de feuille de calcul.

```csharp
public enum SheetType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| VB | `0` | Module Visual Basic |
| Worksheet | `1` |  |
| Chart | `2` | Graphique |
| BIFF4Macro | `3` | Feuille macro BIFF4 |
| InternationalMacro | `4` | Feuille macro internationale |
| Other | `5` |  |
| Dialog | `6` | Feuille de calcul de dialogue |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Insérer une nouvelle feuille de calcul de type Worksheet à l'index 0
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // Définir le nom de la nouvelle feuille de calcul
            newWorksheet.Name = "InsertedSheet";
            
            // Accéder aux cellules de la nouvelle feuille de calcul et ajouter des données
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // Enregistrez le classeur
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


