---
title: "Column.GroupLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Column. Obtient le niveau de groupe de la colonne"
type: docs
url: /fr/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Obtient le niveau de groupe de la colonne.

```csharp
public byte GroupLevel { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Regrouper les colonnes (paramètre isHidden défini sur false)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Obtenir le niveau de groupe de la première colonne
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // Afficher le niveau de groupe
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // Enregistrez le classeur
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


