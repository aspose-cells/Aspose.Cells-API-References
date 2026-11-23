---
title: "Cells.Subtotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Crée des sous-totaux pour la plage"
type: docs
url: /fr/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Crée des sous‑totaux pour la plage.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | La plage |
| groupBy | Int32 | Le champ à regrouper, sous forme d'un décalage entier basé à zéro |
| fonction | ConsolidationFunction | La fonction de sous‑total. |
| totalList | Int32[] | Un tableau de décalages de champ à base zéro, indiquant les champs auxquels les sous‑totaux sont ajoutés. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple pour le sous-total
            CreateSampleData(worksheet);

            // Définir la zone de cellules contenant les données (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // Appeler la méthode Subtotal avec les paramètres :
                // - Regrouper par la colonne 0 (Région)
                // - Utiliser la fonction SOMME
                // - Appliquer à la colonne 2 (Ventes)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // Les méthodes ExpandColumnLevel et ExpandRowLevel ont été supprimées pour corriger les erreurs de compilation
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Créer la ligne d'en-tête
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // Créer les lignes de données
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // Remplir les données à partir de la ligne 2 (indice basé zéro 1)
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Crée des sous‑totaux pour la plage.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | La plage |
| groupBy | Int32 | Le champ à regrouper, sous forme d'un décalage entier basé à zéro |
| fonction | ConsolidationFunction | La fonction de sous‑total. |
| totalList | Int32[] | Un tableau de décalages de champ à base zéro, indiquant les champs auxquels les sous‑totaux sont ajoutés. |
| remplacer | Boolean | Indique s'il faut remplacer les sous-totaux actuels |
| pageBreaks | Boolean | Indique s'il faut ajouter un saut de page entre les groupes |
| summaryBelowData | Boolean | Indique si un résumé doit être ajouté sous les données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer des données d'exemple pour le sous-total
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // Définir la zone de cellules pour le sous-total (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // Appeler Subtotal avec les paramètres :
                // - Regrouper par la première colonne (indice basé zéro 0)
                // - Utiliser la fonction Somme
                // - Appliquer à la troisième colonne (indice basé zéro 2)
                // - Remplacer les sous-totaux existants, sauts de page entre les groupes, résumé sous les données
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


