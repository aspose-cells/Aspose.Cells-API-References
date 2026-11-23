---
title: "Cell.GetLeafs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtenir toutes les cellules qui font référence à cette cellule directement et qui doivent être mises à jour lorsque cette cellule est modifiée"
type: docs
url: /fr/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Obtenir toutes les cellules qui font référence à cette cellule directement et qui doivent être mises à jour lorsque cette cellule est modifiée.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Valeur de retour

Énumérateur pour énumérer tous les dépendants (Cell)

### Remarques

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.GetDependentsInCalculation(bool) pour obtenir tous les dépendants dans la chaîne de calcul. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2022. Aspose s’excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données et des formules pour créer des dépendances
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Obtenir la cellule qui a des dépendants
                Cell cell = worksheet.Cells["B1"];

                // Appeler GetLeafs pour obtenir toutes les cellules qui font référence à cette cellule directement
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Enregistrez le classeur
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Obtenir toutes les cellules qui seront mises à jour lorsque cette cellule sera modifiée.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| recursive | Boolean | Indique si elle renvoie ces feuilles qui ne font pas référence directement à cette cellule mais qui font référence à d'autres feuilles de cette cellule |

### Valeur de retour

Énumérateur pour énumérer tous les dépendants (Cell)

### Remarques

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.GetDependentsInCalculation(bool) pour obtenir tous les dépendants dans la chaîne de calcul. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2022. Aspose s’excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données avec des formules pour créer des dépendances
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Obtenir la cellule qui a des dépendants
                Cell cell = worksheet.Cells["A1"];

                // Appeler GetLeafs avec le paramètre récursif défini sur true
                IEnumerator leafs = cell.GetLeafs(true);

                // Affichez les résultats
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Enregistrez le classeur
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


