---
title: "CellArea.StartColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CellArea champ. Obtient ou définit la colonne de départ de cette zone"
type: docs
url: /fr/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Obtient ou définit la colonne de départ de cette zone.

```csharp
public int StartColumn;
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez des données initiales
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // Créez un CellArea et définissez son StartColumn
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // Insérez une nouvelle colonne en décalant les cellules existantes vers le bas
            cells.InsertRange(area, ShiftType.Down);

            // Vérifier le résultat
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### Voir aussi

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


