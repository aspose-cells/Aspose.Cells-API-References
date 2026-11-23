---
title: "PivotTableCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTableCollection. Ajoute un nouveau tableau croisé dynamique moderne depuis Excel 2007 à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string) {#add_2}

Ajoute un nouveau PivotTable moderne (depuis Excel 2007) à la position de ligne et de colonne spécifiée de la feuille de calcul avec les options par défaut.

```csharp
public PivotTable Add(string sourceData, string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| cellName | String | Le nom de la cellule du coin supérieur gauche pour la destination du tableau croisé dynamique. |

### Valeur de retour

L'instance du tableau croisé dynamique nouvellement créée.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, PivotTableCreateOptions) {#add_3}

Ajoute un nouveau PivotTable moderne (depuis Excel 2007) à la position de ligne et de colonne spécifiée de la feuille de calcul avec les options par défaut.

```csharp
public PivotTable Add(string sourceData, string cellName, PivotTableCreateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| cellName | String | Le nom de la cellule du coin supérieur gauche pour la destination du tableau croisé dynamique. |
| options | PivotTableCreateOptions | Les options de création du tableau croisé dynamique. |

### Valeur de retour

L'instance du tableau croisé dynamique nouvellement créée.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add}

Ajoute un nouveau PivotTable moderne (depuis Excel 2007) à la position de ligne et de colonne spécifiée de la feuille de calcul avec les options par défaut.

```csharp
public PivotTable Add(string sourceData, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| ligne | Int32 | L'index de ligne basé sur zéro du coin supérieur gauche pour la destination du tableau croisé dynamique. |
| column | Int32 | L'index de colonne basé sur zéro du coin supérieur gauche pour la destination du tableau croisé dynamique. |

### Valeur de retour

L'instance du tableau croisé dynamique nouvellement créée.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, PivotTableCreateOptions) {#add_1}

Ajoute un nouveau PivotTable à la position de ligne et de colonne spécifiée de la feuille de calcul.

```csharp
public PivotTable Add(string sourceData, int row, int column, PivotTableCreateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| ligne | Int32 | L'index de ligne basé sur zéro du coin supérieur gauche pour la destination du tableau croisé dynamique. |
| column | Int32 | L'index de colonne basé sur zéro du coin supérieur gauche pour la destination du tableau croisé dynamique. |
| options | PivotTableCreateOptions | Options de création de tableau croisé dynamique. |

### Valeur de retour

L'instance du tableau croisé dynamique nouvellement créée.

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_9}

Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | Les données pour le cache du nouveau tableau croisé dynamique. |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index dans cette liste de tableaux croisés dynamiques.

### Remarques

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du CSV source
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "SourceData";
            
            // Ajoutez des données d'exemple
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Value");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(10);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(20);
            sourceSheet.Cells["A4"].PutValue("A");
            sourceSheet.Cells["B4"].PutValue(30);

            // Créer une feuille de calcul de tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Obtenir la plage de données source
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
            string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
            
            // Ajouter un tableau croisé dynamique en utilisant les paramètres String, String, String
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
            
            // Configurer le tableau croisé dynamique
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Enregistrez le classeur
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_10}

Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, string, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | Les données pour le cache du nouveau tableau croisé dynamique. |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | Boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela permettra d'économiser de la mémoire. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Remarques

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Définir les paramètres pour la méthode Add
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // Appeler la méthode Add avec les paramètres (String, String, String, Boolean)
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // Configurer le tableau croisé dynamique
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_6}

Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| ligne | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index dans cette liste de tableaux croisés dynamiques.

### Remarques

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul pour les données
            Worksheet dataWorksheet = workbook.Worksheets[0];
            dataWorksheet.Name = "Data";
            
            // Ajoutez des données d'exemple
            dataWorksheet.Cells["A1"].PutValue("Category");
            dataWorksheet.Cells["B1"].PutValue("Product");
            dataWorksheet.Cells["C1"].PutValue("Sales");
            
            dataWorksheet.Cells["A2"].PutValue("Electronics");
            dataWorksheet.Cells["B2"].PutValue("Laptop");
            dataWorksheet.Cells["C2"].PutValue(1000);
            
            dataWorksheet.Cells["A3"].PutValue("Electronics");
            dataWorksheet.Cells["B3"].PutValue("Phone");
            dataWorksheet.Cells["C3"].PutValue(800);
            
            dataWorksheet.Cells["A4"].PutValue("Furniture");
            dataWorksheet.Cells["B4"].PutValue("Chair");
            dataWorksheet.Cells["C4"].PutValue(200);
            
            // Ajouter une feuille de calcul pour le tableau croisé dynamique
            Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
            
            // Ajouter un tableau croisé dynamique en utilisant la méthode Add avec les paramètres (String, Int32, Int32, String)
            string pivotDataRange = "Data!A1:C4";
            int row = 0;
            int column = 0;
            string tableName = "SalesPivotTable";
            
            int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
            
            // Accéder au tableau croisé dynamique
            PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Définir la fonction de consolidation
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
            
            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_7}

Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| ligne | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | Boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela permettra d'économiser de la mémoire. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Remarques

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // Définir la plage de données
            string sourceData = "A1:C4";
            
            try
            {
                // Appeler la méthode Add avec les paramètres : (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // Accéder au tableau croisé dynamique nouvellement créé
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configurer le tableau croisé dynamique
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_8}

Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| ligne | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | Boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela permettra d'économiser de la mémoire. |
| isXlsClassic | Boolean | Indique si l'ajout d'un tableau croisé dynamique classique d'Excel 97-2003. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Remarques

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après octobre 2026. Nous nous excusons pour tout inconvénient.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // Définir la plage de données source
            string sourceData = "A1:C5";

            try
            {
                // Appelez la méthode Add avec les paramètres (String, Int32, Int32, String, Boolean, Boolean)
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // Configurer le tableau croisé dynamique
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_11}

Ajoute un nouveau tableau croisé dynamique.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| cellule | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | Boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela permettra d'économiser de la mémoire lorsque la même source de données est regroupée dans un cache de tableau croisé dynamique. |
| isXlsClassic | Boolean | Indique si l'ajout d'un tableau croisé dynamique classique d'Excel 97-2003. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Remarques

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après octobre 2026. Nous nous excusons pour tout inconvénient.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplissez des données d'exemple
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                cells["A" + i].PutValue("Cat" + (i % 3 + 1));
                cells["B" + i].PutValue("Prod" + i);
                cells["C" + i].PutValue(i * 100);
            }

            // Ajouter un tableau croisé dynamique avec les paramètres spécifiés
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
            
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Ajoute un nouveau PivotTable basé sur un autre PivotTable.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Le tableau croisé dynamique source. |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau tableau croisé dynamique ajouté.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Créer un tableau croisé dynamique à partir de la plage de données
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // Appelez la méthode Add avec les paramètres (PivotTable, String, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Enregistrer le classeur pour montrer l'effet
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_4}

Ajoute un nouveau PivotTable basé sur un autre PivotTable.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Le tableau croisé dynamique source. |
| ligne | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau tableau croisé dynamique ajouté.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Créer un tableau croisé dynamique source
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Appelez la méthode Add avec les paramètres (PivotTable, Int32, Int32, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Enregistrer le classeur pour montrer l'effet
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_13}

Ajoute un nouvel objet PivotTable à la collection avec plusieurs plages de consolidation comme source de données.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String[] | Les multiples plages de consolidation, telles que {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Indique si un champ de page unique est créé automatiquement. Si vrai, le paramètre suivant pageFields sera ignoré. |
| pageFields | PivotPageFields | Les éléments du champ de page du tableau croisé dynamique. |
| destCellName | String | destCellName Le nom du nouveau rapport de tableau croisé dynamique. |
| tableName | String | le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau tableau croisé dynamique ajouté.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // Définir la plage de données
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // Appelez la méthode Add avec les paramètres spécifiés
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Accéder au tableau croisé dynamique nouvellement créé
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configurer les champs du tableau croisé dynamique
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_12}

Ajoute un nouvel objet PivotTable à la collection avec plusieurs plages de consolidation comme source de données.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String[] | Les multiples plages de consolidation, telles que {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Indique si un champ de page unique est créé automatiquement. Si vrai, le paramètre suivant pageFields sera ignoré |
| pageFields | PivotPageFields | Les éléments du champ de page du tableau croisé dynamique. |
| ligne | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport du tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau tableau croisé dynamique ajouté.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // Définir les paramètres pour la méthode Add
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // Appelez la méthode Add avec les paramètres spécifiés
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Configurer le tableau croisé dynamique
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // Rafraîchir les données
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


