---
title: "Cell.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient le numéro de colonne basé sur zéro de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/column/
---
## Cell.Column property

Obtient le numéro de colonne (à partir de zéro) de la cellule.

```csharp
public int Column { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez aux cellules et démontrez la propriété Column
            Cell cell1 = worksheet.Cells["A1"];
            Cell cell2 = worksheet.Cells["B2"];
            Cell cell3 = worksheet.Cells["C3"];

            // Définissez les valeurs et les styles
            cell1.PutValue("Cell A1");
            cell2.PutValue("Cell B2");
            cell3.PutValue("Cell C3");

            // Démontrez l’utilisation de la propriété Column
            Console.WriteLine("Cell A1 is in column: " + cell1.Column);
            Console.WriteLine("Cell B2 is in column: " + cell2.Column);
            Console.WriteLine("Cell C3 is in column: " + cell3.Column);

            // Modifiez la largeur de la colonne en utilisant la propriété Column
            worksheet.Cells.Columns[cell1.Column].Width = 20;
            worksheet.Cells.Columns[cell2.Column].Width = 25;
            worksheet.Cells.Columns[cell3.Column].Width = 30;

            // Enregistrez le classeur
            workbook.Save("ColumnPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


