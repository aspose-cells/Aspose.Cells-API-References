---
title: "Worksheet.CalculateArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Calcule une formule en tant que formule de tableau"
type: docs
url: /fr/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Calcule une formule en tant que formule matricielle.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | Formule à calculer. |
| opts | CalculationOptions | Options pour le calcul de la formule |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Définir une formule de tableau
            string arrayFormula = "=SUM(A1:B3)";
            
            // Calculer la formule de tableau avec des options de calcul
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // Afficher le résultat
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Calcule une formule en tant que formule matricielle.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | Formule à calculer. |
| opts | CalculationOptions | Options pour le calcul de la formule |
| maxRowCount | Int32 | le nombre maximal de lignes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de lignes sera utilisé. |
| maxColumnCount | Int32 | le nombre maximal de colonnes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de colonnes sera utilisé. |

### Valeur de retour

Résultat de la formule calculée.

### Remarques

La formule sera considérée comme une formule de tableau dynamique pour calculer la dimension et le résultat. La dimension maximale spécifiée par l'utilisateur est utilisée dans les cas où le résultat calculé constitue un grand ensemble de données (par exemple, le résultat calculé peut correspondre à une ligne ou une colonne entière) mais l'utilisateur n'a pas besoin d'un tableau aussi grand selon les exigences métier ou pour des considérations de performance.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // Créer un classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exemple 1 : Calcul simple d'une formule de tableau
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // Exemple 2 : Formule de tableau avec plage dynamique
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // Exemple 3 : Formule de tableau avec la fonction MATCH
            // Configurer des données de test
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Calcule une formule en tant que formule matricielle.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | Formule à calculer. |
| pOpts | FormulaParseOptions | Options pour analyser la formule |
| cOpts | CalculationOptions | Options pour le calcul de la formule |
| baseCellRow | Int32 | L'index de ligne de la cellule de base. |
| baseCellColumn | Int32 | L'index de colonne de la cellule de base. |
| maxRowCount | Int32 | Le nombre maximal de lignes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de lignes sera utilisé. |
| maxColumnCount | Int32 | Le nombre maximal de colonnes des données résultantes. S'il est non positif ou supérieur au nombre réel de lignes, alors le nombre réel de colonnes sera utilisé. |
| calculationData | CalculationData | Les données de calcul. Elles sont utilisées dans le cas où l'utilisateur doit calculer des formules statiques lors de la mise en œuvre d'un moteur de calcul personnalisé. Pour ce type de situation, l'utilisateur doit les spécifier avec les données de calcul fournies pour [`Calculate`](../../abstractcalculationengine/calculate/). |

### Valeur de retour

Résultat de la formule calculée.

### Remarques

La formule sera considérée comme une formule de tableau dynamique pour calculer la dimension et le résultat. La dimension maximale spécifiée par l'utilisateur est utilisée dans les cas où le résultat calculé constitue un grand ensemble de données (par exemple, le résultat calculé peut correspondre à une ligne ou une colonne entière) mais l'utilisateur n'a pas besoin d'un tableau aussi grand selon les exigences métier ou pour des considérations de performance.

### Voir aussi

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


