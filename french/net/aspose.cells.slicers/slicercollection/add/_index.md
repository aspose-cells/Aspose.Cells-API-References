---
title: "SlicerCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SlicerCollection. Ajoutez un nouveau Slicer en utilisant PivotTable comme source de données"
type: docs
url: /fr/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldName | String | Le nom du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // Ajouter un slicer
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| ligne | Int32 | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| column | Int32 | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldName | String | Le nom du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Fruit");
            cells["B1"].PutValue("Quantity");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(50);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(30);

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un slicer
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivotTable, 20, 12, "fruit");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| ligne | Int32 | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| column | Int32 | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldIndex | Int32 | L'index du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajoutez un slicer pour la table pivot
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldIndex | Int32 | L'index du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Ajouter un slicer
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| ligne | Int32 | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| column | Int32 | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseField | PivotField | Le PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Ajouter des champs pivot
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un slicer
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Enregistrez le classeur
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseField | PivotField | Le PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // Ajouter un slicer
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // Enregistrez le classeur
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| table | ListObject | Objet ListObject |
| indice | Int32 | L'indice de ListColumn dans ListObject.ListColumns |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage du Slicer. |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez des données d'exemple et un ListObject
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Ajoutez un slicer pour le ListObject - note : Slicers.Add renvoie un indice int
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Enregistrez le classeur
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| table | ListObject | Objet ListObject |
| listColumn | ListColumn | Le ListColumn dans ListObject.ListColumns |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage du Slicer. |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");

            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, table.ListColumns[1], "I38");

            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells.SetColumnWidth(1, 20);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| table | ListObject | Objet ListObject |
| listColumn | ListColumn | Le ListColumn dans ListObject.ListColumns |
| ligne | Int32 | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| column | Int32 | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |

### Valeur de retour

Le nouvel indice d'ajout du Slicer

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple pour le tableau
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue("CatA");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue("CatB");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue("CatA");
            
            // Créez la plage du tableau
            int endRow = 4;
            string startCell = "A1";
            string endCell = $"B{endRow}";
            
            // Ajoutez le tableau à la feuille de calcul en utilisant la surcharge correcte
            int tableIndex = sheet.ListObjects.Add(startCell, endCell, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Ajoutez un slicer pour la colonne Category à la position (ligne 6, colonne 1)
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(table, table.ListColumns[1], 6, 1);
            
            // Enregistrer le résultat
            workbook.Save("SlicerOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


