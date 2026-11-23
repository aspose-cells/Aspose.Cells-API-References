---
title: "Cell.SetTableFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Créer un tableau de données à deux variables pour la plage donnée en commençant à partir de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Créer un tableau de données à deux variables pour la plage donnée en commençant à partir de cette cellule.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |
| rowInputCell | String | la cellule d'entrée de ligne |
| columnInputCell | String | la cellule d'entrée de colonne |
| valeurs | Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // Cellule cible où la formule du tableau sera définie
            Cell targetCell = worksheet.Cells["C3"];

            // Préparer les paramètres pour SetTableFormula
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Définir la formule du tableau sur la cellule cible
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Calculer les formules du classeur pour actualiser les résultats
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Créer un tableau de données à une variable pour la plage donnée en commençant à partir de cette cellule.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |
| inputCell | String | la cellule d'entrée |
| isRowInput | Boolean | Indique si la cellule d'entrée est une cellule d'entrée de ligne (true) ou une cellule d'entrée de colonne (false). |
| valeurs | Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // Préparer les paramètres pour SetTableFormula
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // Obtenir la cellule cible pour le tableau de données (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // Appeler SetTableFormula avec des variations de taux d'intérêt
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // Calculer les formules pour actualiser les résultats du tableau
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Créer un tableau de données à deux variables pour la plage donnée en commençant à partir de cette cellule.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |
| rowIndexOfRowInputCell | Int32 | indice de ligne de la cellule d'entrée de ligne |
| columnIndexOfRowInputCell | Int32 | indice de colonne de la cellule d'entrée de ligne |
| rowIndexOfColumnInputCell | Int32 | indice de ligne de la cellule d'entrée de colonne |
| columnIndexOfColumnInputCell | Int32 | indice de colonne de la cellule d'entrée de colonne |
| valeurs | Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // Préparer les valeurs d'entrée pour le tableau de données (taux d'intérêt et montants de prêt)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // Définir la formule du tableau avec des dimensions de tableau de données 3x3 et des décalages de cellule d'entrée
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Créer un tableau de données à une variable pour la plage donnée en commençant à partir de cette cellule.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Nombre de lignes à remplir dans la formule. |
| columnNumber | Int32 | Nombre de colonnes à remplir dans la formule. |
| rowIndexOfInputCell | Int32 | indice de ligne de la cellule d'entrée |
| columnIndexOfInputCell | Int32 | indice de colonne de la cellule d'entrée |
| isRowInput | Boolean | Indique si la cellule d'entrée est une cellule d'entrée de ligne (true) ou une cellule d'entrée de colonne (false). |
| valeurs | Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // Créer un tableau de données d'exemple pour les paramètres de la formule du tableau
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Obtenir la cellule cible pour appliquer la formule du tableau
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // Définir la formule du tableau avec : 
                // 3 lignes, 2 colonnes, cellule d'entrée à A1 (0,0), 
                // type d'entrée de ligne, et valeurs d'exemple
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


