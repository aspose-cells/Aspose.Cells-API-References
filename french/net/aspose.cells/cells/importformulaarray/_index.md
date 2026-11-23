---
title: "Cells.ImportFormulaArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Importe un tableau de formules dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/importformulaarray/
---
## Cells.ImportFormulaArray method

Importe un tableau de formules dans une feuille de calcul.

```csharp
public void ImportFormulaArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stringArray | String[] | Tableau de formules. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| isVertical | Boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Préparer le tableau de formules et les paramètres
            string[] formulas = new string[] { "=A1+B1", "=C1*D1" };
            int firstRow = 0;
            int firstColumn = 0;
            bool isVertical = true;

            try
            {
                // Importer les formules verticalement à partir de la cellule A1
                worksheet.Cells.ImportFormulaArray(formulas, firstRow, firstColumn, isVertical);
                
                // Définir les valeurs pour les références de formules
                worksheet.Cells["A1"].PutValue(2);
                worksheet.Cells["B1"].PutValue(3);
                worksheet.Cells["C1"].PutValue(4);
                worksheet.Cells["D1"].PutValue(5);
                
                // Calculer les formules
                workbook.CalculateFormula();

                Console.WriteLine("Formulas imported successfully. Calculated results:");
                Console.WriteLine($"A2 value: {worksheet.Cells["A2"].Value}"); // Should be 5
                Console.WriteLine($"A3 value: {worksheet.Cells["A3"].Value}"); // Should be 20
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportFormulaArray method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


