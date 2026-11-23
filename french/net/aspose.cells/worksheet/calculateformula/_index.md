---
title: "Worksheet.CalculateFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Calcule une formule"
type: docs
url: /fr/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Calcule une formule.

```csharp
public object CalculateFormula(string formula)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | Formule à calculer. |

### Valeur de retour

Résultat de la formule calculée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // Démontrer la conversion de nombres de base
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // Démontrer la conversion de devises
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // Démontrer la conversion de temps
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // Démontrer la conversion de dates
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // Démontrer le cas d'erreur
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Calcule directement une expression de formule.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | Formule à calculer. |
| opts | CalculationOptions | Options pour le calcul de la formule |

### Valeur de retour

Résultat calculé de la formule donnée. L'objet retourné peut être de types possibles de [`Value`](../../cell/value/), ou ReferredArea.

### Remarques

La formule sera calculée exactement comme si elle avait été définie dans la cellule A1. Et la formule sera considérée comme une formule normale. Si vous avez besoin que la formule soit calculée comme une formule matricielle et d'obtenir un tableau pour le résultat calculé, veuillez utiliser [`CalculateArrayFormula`](../calculatearrayformula/) à la place.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Créez un moteur de calcul personnalisé
            CustomEngine customEngine = new CustomEngine();
            
            // Calculer la formule en utilisant le moteur personnalisé
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
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

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Calcule directement une expression de formule.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | Formule à calculer. |
| pOpts | FormulaParseOptions | Options pour l'analyse de la formule. |
| cOpts | CalculationOptions | Options pour le calcul de la formule. |
| baseCellRow | Int32 | L'index de ligne de la cellule de base. |
| baseCellColumn | Int32 | L'index de colonne de la cellule de base. |
| calculationData | CalculationData | Les données de calcul. Elles sont utilisées dans le cas où l'utilisateur doit calculer des formules statiques lors de la mise en œuvre d'un moteur de calcul personnalisé. Pour ce type de situation, l'utilisateur doit les spécifier avec les données de calcul fournies pour [`Calculate`](../../abstractcalculationengine/calculate/). |

### Valeur de retour

Résultat calculé de la formule donnée. L'objet retourné peut être de types possibles de [`Value`](../../cell/value/), ou ReferredArea.

### Remarques

La formule sera calculée exactement comme si elle était définie dans la cellule de base spécifiée. Et la formule sera traitée comme une formule normale. Si vous avez besoin que la formule soit calculée comme une formule matricielle et d'obtenir un tableau pour le résultat calculé, veuillez utiliser [`CalculateArrayFormula`](../calculatearrayformula/) à la place.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplissez des données d'exemple
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // Définir les options de calcul
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // Définir les options d'analyse de formule
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // Calculer la formule avec tous les paramètres
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // Afficher le résultat
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Voir aussi

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Calcule toutes les formules de cette feuille de calcul.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options de calcul |
| recursive | Boolean | True signifie que si les cellules de la feuille de calcul dépendent des cellules d'autres feuilles de calcul, les cellules dépendantes dans les autres feuilles seront également calculées. False signifie que toutes les formules de la feuille de calcul ont été calculées et que les valeurs sont correctes. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple et des formules
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // Créer des options de calcul
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // Calculer la formule avec des options et forcer le calcul complet
            worksheet.CalculateFormula(options, true);
            
            // Afficher le résultat calculé
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


