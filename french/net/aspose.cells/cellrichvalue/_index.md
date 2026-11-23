---
title: "Classe CellRichValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellRichValue. Représente la valeur riche de la cellule"
type: docs
url: /fr/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Représente la valeur enrichie de la cellule.

```csharp
public abstract class CellRichValue
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Obtient le texte alternatif associé à l'image. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Obtient le type de valeur d'erreur de la cellule. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Obtient les données d'image de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir une valeur riche dans la cellule A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // Obtenir la valeur riche de la cellule A1
            CellRichValue richValue = cell.GetRichValue();
            
            // Afficher les propriétés de la valeur riche
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Enregistrez le classeur
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


