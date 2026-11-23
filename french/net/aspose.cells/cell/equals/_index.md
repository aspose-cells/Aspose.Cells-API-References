---
title: "Cell.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Vérifie si cet objet fait référence à la même cellule qu'un autre"
type: docs
url: /fr/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

Vérifie si cet objet fait référence à la même cellule qu'un autre.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | un autre objet |

### Valeur de retour

true si deux objets font référence à la même cellule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder aux cellules depuis différents emplacements
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // Définir des valeurs identiques dans différentes cellules
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // Comparer les mêmes références de cellules physiques
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // Comparer différentes cellules avec un contenu identique
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // Comparer une cellule avec un objet non‑cellule
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule.

```csharp
public bool Equals(Cell cell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellule | Cellule | un autre objet cellule |

### Valeur de retour

vrai si deux objets cellule font référence à la même cellule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des cellules à différents emplacements (A1 et B1)
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // Définir des valeurs identiques dans les deux cellules
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // Comparer cellA1 avec cellB1 (emplacements différents)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // Comparer cellA1 avec elle-même (même instance)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


