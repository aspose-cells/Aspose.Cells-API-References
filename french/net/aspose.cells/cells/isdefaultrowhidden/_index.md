---
title: "Cells.IsDefaultRowHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Indique si la ligne est masquée par défaut"
type: docs
url: /fr/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Indique si la ligne est masquée par défaut.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la propriété de ligne masquée par défaut
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // Afficher la valeur actuelle de IsDefaultRowHidden
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


