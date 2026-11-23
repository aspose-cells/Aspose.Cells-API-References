---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Actualise les débordements de formules de tableau dynamique dans une nouvelle plage de cellules voisines selon les données actuelles. Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules de tableau dynamique."
type: docs
url: /fr/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Actualise les formules de tableau dynamique(débordent dans une nouvelle plage de cellules voisines selon les données actuelles) Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules de tableau dynamique.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| calculer | Boolean | Indique si les valeurs des cellules sont calculées et mises à jour pour ces formules de tableau dynamique |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // Configurer les données initiales et les formules de tableau dynamique
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // Modifier la plage et actualiser les formules
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Actualise les formules de tableau dynamique(débordent dans une nouvelle plage de cellules voisines selon les données actuelles)

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| calculer | Boolean | Indique si les valeurs des cellules sont calculées et mises à jour pour ces formules de tableau dynamique |
| copts | CalculationOptions | Les options de calcul des formules |

### Remarques

Pour des raisons de performance, nous n'actualisons pas automatiquement toutes les formules de tableau dynamique lorsque la formule elle‑même ou les données auxquelles elle fait référence sont modifiées. L'utilisateur doit donc appeler cette méthode manuellement après les opérations susceptibles d'influencer les formules de tableau dynamique, telles que l'importation/ la définition de valeurs de cellules, l'insertion/la suppression de lignes/colonnes/plages, etc. Pour la plupart des formules contenant des fonctions, le calcul de la plage de débordement nécessite également le calcul de la formule, ainsi, en général, la valeur true du drapeau "calculate" est préférée. Si la formule est simple, comme une référence de plage ou un tableau (par exemple "=C1:E5", "={1,2;3,4}", ...), une fonction simple sur une plage ou un tableau (par exemple "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), et que toutes les formules seront calculées ultérieurement (par exemple via [`CalculateFormula`](../calculateformula/)), alors l'utilisation de la valeur false pour le drapeau "calculate" peut éviter le calcul dupliqué au profit des performances.

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un exemple de formule de tableau dynamique
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // Créer des options de calcul
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // Actualiser les formules de tableau dynamique avec les options de calcul
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // Calculer les formules du classeur
            workbook.CalculateFormula(opts);
            
            // Afficher le résultat de A1:A5
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


