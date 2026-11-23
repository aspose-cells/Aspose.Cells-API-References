---
title: "WorksheetCollection.CreateUnionRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Crée un objet Range à partir d'une adresse de la plage"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Crée un objet [`Range`](../../range/) à partir d'une adresse de la plage.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| address | String | L'adresse de la plage. |
| sheetIndex | Int32 | L'index de la feuille. |

### Valeur de retour

Un objet [`Range`](../../range/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage d'union à partir de chaînes d'adresses
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Définit la valeur pour l'ensemble de la plage d'union
            unionRange.Value = "Test";
            
            // Appliquer le style à la plage d'union
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // Enregistrez le classeur
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


