---
title: "Cells.ImportArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells."
type: docs
url: /fr/net/aspose.cells/cells/importarray/
---
## ImportArray(string[], int, int) {#importarray_4}

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn)
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(string[], int, int, bool) {#importarray_5}

Importe un tableau de chaînes dans une feuille de calcul.

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stringArray | String[] | Tableau de chaînes. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| isVertical | Boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données du tableau de chaînes
            string[] fruitArray = new string[] { "Apple", "Banana", "Cherry", "Date", "Elderberry" };

            try
            {
                // Appeler ImportArray avec les paramètres : (String[], Int32, Int32, Boolean)
                // Commencer l'importation à la ligne 2 (3e ligne), colonne 1 (colonne B), verticalement
                worksheet.Cells.ImportArray(fruitArray, 2, 1, true);

                Console.WriteLine("Imported string array vertically starting from cell B3:");
                foreach (string fruit in fruitArray)
                {
                    Console.WriteLine(fruit);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("CellsMethodImportArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int) {#importarray_2}

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn)
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int, bool) {#importarray_3}

Importe un tableau d'entiers dans une feuille de calcul.

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| intArray | Int32[] | Tableau d'entiers. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| isVertical | Boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithInt32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données du tableau Int32
            int[] data = new int[] { 1, 2, 3, 4, 5 };

            try
            {
                // Appeler ImportArray avec les paramètres : (Int32[], firstRow=2, firstColumn=1, isVertical=true)
                worksheet.Cells.ImportArray(data, 2, 1, true);

                Console.WriteLine("Imported array vertically starting from cell B3:");
                for (int i = 0; i < data.Length; i++)
                {
                    Console.WriteLine($"Cell B{3 + i}: {worksheet.Cells[2 + i, 1].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("CellsMethodImportArrayWithInt32Int32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int) {#importarray}

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn)
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int, bool) {#importarray_1}

Importe un tableau de doubles dans une feuille de calcul.

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| doubleArray | Double[] | Tableau de doubles. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| isVertical | Boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithDoubleInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Préparer des données d'exemple pour le tableau de doubles
            double[] dataArray = new double[] { 1.23, 4.56, 7.89, 10.11, 12.13 };
            const int targetRow = 2;    // 0-based row index (3rd row)
            const int targetColumn = 1; // 0-based column index (2nd column)
            const bool isVertical = true;

            try
            {
                // Obtenir la collection de cellules et appeler ImportArray
                Cells cells = worksheet.Cells;
                cells.ImportArray(dataArray, targetRow, targetColumn, isVertical);
                
                Console.WriteLine($"Imported {dataArray.Length} double values starting at row {targetRow + 1}, column {targetColumn + 1}");
                Console.WriteLine($"Data orientation: {(isVertical ? "Vertical" : "Horizontal")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("CellsImportArrayDoubleVerticalDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


