---
title: "Cell.SetSharedFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Définit une formule pour une plage de cellules"
type: docs
url: /fr/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Définit une formule pour une plage de cellules.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Formule partagée. |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |
| isR1C1 | Boolean | si la formule est au format R1C1 |
| isLocal | Boolean | si la formule est formatée selon la locale |

### Remarques

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Cette propriété sera supprimée 12 mois plus tard à compter de décembre 2019. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // Remplir des données d'exemple dans la colonne A
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // Obtenir la cellule cible B1 pour définir la formule partagée
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // Définir la formule partagée pour calculer le carré des valeurs dans la colonne A
                // Paramètres : (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // Vérifier la propagation de la formule
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // Calculer le classeur pour actualiser les résultats de la formule
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // Enregistrer le classeur modifié
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Définit des formules partagées pour une plage de cellules.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Formule partagée. |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir une formule partagée dans la colonne B à partir de B1 jusqu'à B20
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // Définir quelques valeurs dans la colonne C pour démontrer le calcul de la formule
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // Calculer les formules
            workbook.CalculateFormula();

            // Afficher les résultats pour vérification
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Définit des formules partagées pour une plage de cellules.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Formule partagée. |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |
| options | FormulaParseOptions | Options pour analyser la formule. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple dans la colonne A
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Obtenir la cellule cible où nous définirons la formule partagée
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // Créer des options d'analyse de formule avec les paramètres par défaut
                FormulaParseOptions options = new FormulaParseOptions();

                // Définir la formule partagée pour 3 lignes et 2 colonnes à partir de B1
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Définit des formules partagées pour une plage de cellules.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Formule partagée. |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |
| options | FormulaParseOptions | Options pour analyser la formule. |
| valeurs | Object[][] | valeurs pour ces cellules avec la formule partagée donnée |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la valeur d'exemple dans la cellule A1
            worksheet.Cells["A1"].PutValue(5);

            // Obtenir la cellule cible B2 où la formule partagée sera définie
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // Définir les paramètres de la formule partagée
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // Définir la formule partagée pour la plage 2x2 commençant à B2 avec des valeurs prédéfinies
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


