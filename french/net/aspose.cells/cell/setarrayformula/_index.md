---
title: "Cell.SetArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Définit une formule matricielle pour une plage de cellules"
type: docs
url: /fr/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Définit une formule de tableau pour une plage de cellules.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Formule matricielle. |
| rowNumber | Int32 | Nombre de lignes à remplir avec le résultat de la formule matricielle. |
| columnNumber | Int32 | Nombre de colonnes à remplir avec le résultat de la formule matricielle. |
| isR1C1 | Boolean | si la formule est au format R1C1 |
| isLocal | Boolean | si la formule est formatée selon la locale |

### Remarques

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2019. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // Obtenir la cellule cible où nous voulons définir la formule matricielle
                Cell targetCell = worksheet.Cells["B1"];

                // Définir une formule matricielle qui multiplie les valeurs de A1:A3 par 2
                // Paramètres : (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // Calculer le classeur pour voir les résultats
                workbook.CalculateFormula();

                // Affichez les résultats
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // Enregistrez le classeur
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

Définit une formule de tableau(formule de tableau héritée saisie via CTRL+SHIFT+ENTER dans MS Excel) pour une plage de cellules.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Formule matricielle. |
| rowNumber | Int32 | Nombre de lignes à remplir avec le résultat de la formule matricielle. |
| columnNumber | Int32 | Nombre de colonnes à remplir avec le résultat de la formule matricielle. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Définit une formule de tableau pour une plage de cellules.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Formule matricielle. |
| rowNumber | Int32 | Nombre de lignes à remplir avec le résultat de la formule matricielle. |
| columnNumber | Int32 | Nombre de colonnes à remplir avec le résultat de la formule matricielle. |
| options | FormulaParseOptions | Options pour analyser la formule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Placer des données d'exemple dans les cellules C1:E1
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // Définir une formule matricielle dans la cellule A1 qui s'étendra sur 2 lignes et 3 colonnes
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // Calculer les formules
            workbook.CalculateFormula();

            // Afficher les résultats
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
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

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Définit une formule de tableau pour une plage de cellules.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Formule matricielle. |
| rowNumber | Int32 | Nombre de lignes à remplir avec le résultat de la formule matricielle. |
| columnNumber | Int32 | Nombre de colonnes à remplir avec le résultat de la formule matricielle. |
| options | FormulaParseOptions | Options pour analyser la formule. |
| valeurs | Object[][] | valeurs pour ces cellules avec la formule matricielle donnée |

### Voir aussi

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


