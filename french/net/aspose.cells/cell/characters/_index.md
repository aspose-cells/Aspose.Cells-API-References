---
title: "Cell.Characters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Retourne un objet Characters qui représente une plage de caractères dans le texte de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/characters/
---
## Cell.Characters method

Renvoie un objet Characters qui représente une plage de caractères dans le texte de la cellule.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index du début du caractère. |
| longueur | Int32 | Le nombre de caractères. |

### Valeur de retour

Objet Characters.

### Remarques

Cette méthode ne fonctionne que sur une cellule contenant une valeur de chaîne.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


