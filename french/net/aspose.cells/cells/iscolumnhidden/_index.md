---
title: "Cells.IsColumnHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Vérifie si une colonne à l’indice donné est masquée"
type: docs
url: /fr/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Vérifie si une colonne à l'index donné est masquée.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | indice de colonne |

### Valeur de retour

vrai si la colonne est masquée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Masquez la colonne C (index 2)
            cells.HideColumn(2);
            
            // Vérifiez si la colonne C est masquée
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


