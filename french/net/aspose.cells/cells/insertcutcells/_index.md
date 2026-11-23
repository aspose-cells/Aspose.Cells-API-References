---
title: "Cells.InsertCutCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Insérer la plage découpée"
type: docs
url: /fr/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Insérer la plage découpée.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cutRange | Plage | La plage découpée. |
| ligne | Int32 | La ligne. |
| column | Int32 | La colonne. |
| shiftType | ShiftType | Indique comment déplacer les autres objets de la plage cible lors de l’insertion de la plage découpée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul et à ses cellules
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // Ajoutez des données aux cellules source
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // Créez une deuxième feuille de calcul comme destination
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // Ajoutez des données initiales à la destination
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // Créez une plage à découper (A1:B2 de la feuille source)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // Insérez les cellules découpées en B2 dans la feuille de destination, en décalant les cellules vers le bas
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // Enregistrez le classeur
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


