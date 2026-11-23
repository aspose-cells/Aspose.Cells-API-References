---
title: "Cells.MaxDataRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Indice de ligne maximal de la cellule contenant des données"
type: docs
url: /fr/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Indice de ligne maximal de la cellule contenant des données.

```csharp
public int MaxDataRow { get; }
```

### Remarques

Renvoie -1 s'il n'y a aucune cellule contenant des données. Cette propriété doit itérer et vérifier les cellules et les lignes dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // Démontrer l'utilisation de MaxDataRow
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // Créer une zone de cellules en utilisant MaxDataRow
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // Appliquer le formatage à la plage de données
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // Appliquer le style à la plage
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // Enregistrez le classeur
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


