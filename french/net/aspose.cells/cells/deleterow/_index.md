---
title: "Cells.DeleteRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Supprime une ligne"
type: docs
url: /fr/net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

Supprime une ligne.

```csharp
public void DeleteRow(int rowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de la ligne à supprimer. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Définissez une formule partagée dans la ligne 66
            cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);

            // Supprimez la ligne 9 (ce qui décale les lignes vers le haut)
            cells.DeleteRow(9);

            // Vérifiez que la formule a été ajustée après la suppression de la ligne
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
            }

            // Supprimez les lignes 60-61 (ce qui décale les lignes vers le haut)
            cells.DeleteRows(59, 2);

            // Vérifiez que la formule a été ajustée après la suppression des lignes
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRow(int, bool) {#deleterow_1}

Supprime une ligne.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de la ligne à supprimer. |
| updateReference | Boolean | Indique si les références doivent être mises à jour dans les autres feuilles de calcul. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            sheet.Cells.DeleteRow(2, true);

            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            workbook.Save("DeleteRowExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


