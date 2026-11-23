---
title: "Cell.SetDynamicArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible"
type: docs
url: /fr/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | String | l'expression de la formule |
| options | FormulaParseOptions | options pour analyser la formule. L'option "Parse" sera ignorée et la formule sera toujours analysée immédiatement |
| calculateValue | Boolean | si calculer cette formule de tableau dynamique pour ces cellules dans la plage débordée. |

### Valeur de retour

la plage dans laquelle la formule doit se déverser.

### Remarques

la plage renvoyée peut ne pas être identique à celle réelle dans laquelle cette formule de tableau dynamique se déverse. S'il y a des cellules non vides dans la plage, la formule sera définie uniquement pour la cellule actuelle et marquée comme "#SPILL!". Mais pour ce type de situation nous renvoyons toujours la plage complète dans laquelle cette formule doit se déverser.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Définir la formule de tableau dynamique dans la cellule A1
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // Définir la valeur dans B2 qui affectera la formule SEQUENCE
            cells["B2"].PutValue(3);

            // Calculer les formules et rafraîchir les tableaux dynamiques
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // Afficher les résultats de la plage débordée
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | String | l'expression de la formule |
| options | FormulaParseOptions | options pour analyser la formule. L'option "Parse" sera ignorée et la formule sera toujours analysée immédiatement |
| valeurs | Object[][] | valeurs (résultats calculés) pour ces cellules avec la formule de tableau dynamique donnée |
| calculateRange | Boolean | Si calculer la plage débordée pour cette formule de tableau dynamique. Si le paramètre "values" n'est pas nul et que ce drapeau est faux, alors la hauteur de la plage débordée sera values.Length et la largeur sera values[0].Length. |
| calculateValue | Boolean | si calculer cette formule de tableau dynamique pour ces cellules dans la plage débordée lorsque "values" est nul ou que l'élément correspondant dans "values" pour une cellule est nul. |

### Valeur de retour

la plage dans laquelle la formule doit se déverser.

### Remarques

la plage renvoyée peut ne pas être identique à celle réelle dans laquelle cette formule de tableau dynamique se déverse. S'il y a des cellules non vides dans la plage, la formule sera définie uniquement pour la cellule actuelle et marquée comme "#SPILL!". Mais pour ce type de situation nous renvoyons toujours la plage complète dans laquelle cette formule doit se déverser.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // Obtenir la cellule C1 où la formule de tableau dynamique sera définie
            cell = worksheet.Cells["C1"];

            // Définir la formule de tableau dynamique
            string formula = "=A1:B2 * 2";
            
            // Créer des options d'analyse de formule
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Préparer les valeurs pour remplir les cellules de résultat de la formule
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Définir la formule de tableau dynamique avec des valeurs pré-calculées
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Enregistrer le classeur avec les modifications
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | String | l'expression de la formule |
| options | FormulaParseOptions | options pour analyser la formule. L'option "Parse" sera ignorée et la formule sera toujours analysée immédiatement |
| valeurs | Object[][] | valeurs (résultats calculés) pour ces cellules avec la formule de tableau dynamique donnée |
| calculateRange | Boolean | Si calculer la plage débordée pour cette formule de tableau dynamique. Si le paramètre "values" n'est pas nul et que ce drapeau est faux, alors la hauteur de la plage débordée sera values.Length et la largeur sera values[0].Length. |
| calculateValue | Boolean | si calculer cette formule de tableau dynamique pour ces cellules dans la plage débordée lorsque "values" est nul ou que l'élément correspondant dans "values" pour une cellule est nul. |
| copts | CalculationOptions | Les options pour calculer la formule. Généralement, pour des considérations de performance, la propriété [`Recursive`](../../calculationoptions/recursive/) devrait être false. |

### Valeur de retour

la plage dans laquelle la formule doit se déverser.

### Remarques

la plage renvoyée peut ne pas être identique à celle réelle dans laquelle cette formule de tableau dynamique se déverse. S'il y a des cellules non vides dans la plage, la formule sera définie uniquement pour la cellule actuelle et marquée comme "#SPILL!". Mais pour ce type de situation nous renvoyons toujours la plage complète dans laquelle cette formule doit se déverser.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple dans les cellules A2:B5
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Obtenir la cellule cible D1
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // Préparer les paramètres pour SetDynamicArrayFormula
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // Appeler SetDynamicArrayFormula avec des paramètres spécifiques
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


