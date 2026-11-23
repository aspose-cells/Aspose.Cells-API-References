---
title: "Cells.InsertRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Insère une plage de cellules et décale les cellules selon l'option de décalage"
type: docs
url: /fr/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Insère une plage de cellules et décale les cellules selon l'option de décalage.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| zone | CellArea | Déplacer la zone. |
| shiftNumber | Int32 | Nombre de lignes ou de colonnes à insérer. |
| shiftType | ShiftType | Option de déplacement des cellules. |
| updateReference | Boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir des données d'exemple
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // Définir la zone à insérer (lignes 2-3, colonne A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // Insérer la plage en décalant les cellules vers la droite et mettre à jour les références
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // Vérifier l'opération en contrôlant les valeurs
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Insère une plage de cellules et décale les cellules selon l'option de décalage.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| zone | CellArea | Déplacer la zone. |
| shiftType | ShiftType | Option de déplacement des cellules. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplissez quelques données d'exemple
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // Définir la zone de cellules à insérer
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // Insérer la plage et décaler les cellules vers le bas
            cells.InsertRange(area, ShiftType.Down);

            // Enregistrez le classeur
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Insère une plage de cellules et décale les cellules selon l'option de décalage.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| zone | CellArea | Déplacer la zone. |
| shiftNumber | Int32 | Nombre de lignes ou de colonnes à insérer. |
| shiftType | ShiftType | Option de déplacement des cellules. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // Définir la zone de cellules à insérer (cellule unique B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // Insérer la plage en décalant les cellules vers la droite
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // Enregistrez le classeur
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


