---
title: "Cell.InsertText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Insérer des caractères dans la cellule. Si la cellule est richement formatée, cette méthode peut conserver le formatage original"
type: docs
url: /fr/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Insère des caractères dans la cellule. Si la cellule est formatée richement, cette méthode peut conserver le formatage original.

```csharp
public void InsertText(int index, string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice. |
| texte | String | Texte inséré. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à la cellule B3 et définissez la valeur initiale
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // Insérez du texte à la position 6
            cell.InsertText(6, "Inserted");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


