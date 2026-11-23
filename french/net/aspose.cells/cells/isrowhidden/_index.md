---
title: "Cells.IsRowHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Vérifie si une ligne à l'index donné est masquée"
type: docs
url: /fr/net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Vérifie si une ligne à l'index donné est masquée.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | index de ligne |

### Valeur de retour

vrai si la ligne est masquée

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsRowHiddenWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Données d'exemple
            cells[1, 0].PutValue("US");
            cells[2, 0].PutValue("UK");
            cells[3, 0].PutValue("India");
            cells[4, 0].PutValue("UK");
            cells[5, 0].PutValue("India");
            cells[6, 0].PutValue("US");
            
            // Appliquer le filtre
            AutoFilter af = sheet.AutoFilter;
            af.Range = "A1:A1";
            af.Filter(0, "India");
            af.Refresh();
            
            // Vérifier la visibilité de la ligne
            Console.WriteLine("Row Visibility Check:");
            for (int i = 1; i < 7; i++)
            {
                Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


