---
title: "Row.IsHeightMatched"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. La valeur true de cette propriété indique également que la hauteur de la ligne est automatique sans valeur de hauteur personnalisée définie par l'utilisateur."
type: docs
url: /fr/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. La valeur true de cette propriété indique également que la hauteur de la ligne est "automatique" sans valeur de hauteur personnalisée définie par l'utilisateur.

```csharp
public bool IsHeightMatched { get; set; }
```

### Remarques

Lorsque cette propriété est true, si le contenu de cette ligne change, la hauteur de la ligne doit généralement être recalculée (par exemple avec [`AutoFitRows`](../../worksheet/autofitrows/)) pour obtenir le même résultat que celui affiché dans MS Excel lors de l'ouverture du classeur.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez des données d'exemple et un style pour démontrer la correspondance de la hauteur de ligne.
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // Appliquez le retour à la ligne automatique pour forcer l'ajustement de la hauteur.
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Ajustez automatiquement la ligne pour correspondre à la hauteur du contenu.
            worksheet.AutoFitRow(0);
            
            // Vérifiez si la hauteur de la ligne correspond à son contenu.
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


