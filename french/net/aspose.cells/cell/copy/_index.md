---
title: "Cell.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Copie les données d'une cellule source"
type: docs
url: /fr/net/aspose.cells/cell/copy/
---
## Cell.Copy method

Copie les données d'une cellule source.

```csharp
public void Copy(Cell cell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cell | Cell | Objet [`Cell`](../) source. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCopyWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir les valeurs et les styles dans la cellule source
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // Créer la cellule de destination
            Cell destCell = cells["B1"];

            // Copier de la source vers la destination
            destCell.Copy(sourceCell);

            // Vérifier la copie
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


