---
title: "Cell.SetFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Définit la formule et le résultat calculé de la formule"
type: docs
url: /fr/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Définit la formule et la valeur(résultat calculé) de la formule.

```csharp
public void SetFormula(string formula, object value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La formule. |
| valeur | Object | La valeur (résultat calculé) de la formule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la formule avec des paramètres de chaîne et d'objet
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Afficher les valeurs avant le calcul
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Calculer les formules
            workbook.CalculateFormula();

            // Afficher les valeurs après le calcul
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Définit la formule et la valeur(résultat calculé) de la formule.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La formule. |
| options | FormulaParseOptions | Options pour analyser la formule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir une cellule spécifique (B2 dans ce cas)
            Cell cell = worksheet.Cells["B2"];
            
            // Définir quelques valeurs initiales pour la démonstration
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Exemple 1 : Définir une formule simple avec les options d'analyse par défaut
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Exemple 2 : définir la formule avec le style R1C1 en utilisant FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Exemple 3 : définir la formule avec des options d’analyse qui conservent le format R1C1
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Calculez le classeur pour voir les résultats
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### Voir aussi

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Définissez la formule et la valeur de la formule.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La formule. |
| isR1C1 | Boolean | Indique si la formule est une formule R1C1. |
| isLocal | Boolean | Si la formule est formatée selon la locale. |
| valeur | Object | La valeur de la formule. |

### Remarques

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.SetFormula(string,FormulaParseOptions,object). Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2019. Aspose s’excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Obtenez la cellule cible où nous définirons la formule
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Définissez une formule avec tous les paramètres
                // Paramètres : chaîne de formule, isR1C1, isLocal, valeur
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Calculer la formule
                workbook.CalculateFormula();

                // Afficher le résultat
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Enregistrez le classeur
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
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

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Définit la formule et la valeur(résultat calculé) de la formule.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La formule. |
| options | FormulaParseOptions | Options pour analyser la formule. |
| valeur | Object | La valeur (résultat calculé) de la formule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Définissez la formule initiale avec la référence du module complémentaire
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Utilisez SetFormula pour remplacer sans vérifier le module complémentaire
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Réinitialisez à la formule du module complémentaire
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Créez un nouveau classeur et copiez la feuille
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### Voir aussi

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


