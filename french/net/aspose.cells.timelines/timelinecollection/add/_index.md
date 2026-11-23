---
title: "TimelineCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TimelineCollection. Ajouter une nouvelle chronologie en utilisant PivotTable comme source de données"
type: docs
url: /fr/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| ligne | Int32 | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| column | Int32 | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseFieldName | String | Le nom du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout de la Timeline

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // Ajouter la timeline connectée au tableau croisé dynamique
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // Enregistrer le classeur
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| destCellName | String | Le nom de la cellule dans le coin supérieur gauche de la plage Timeline. |
| baseFieldName | String | Le nom du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout de la Timeline

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // Ajouter un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Ajouter la timeline connectée au tableau croisé dynamique
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // Enregistrez le classeur
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| ligne | Int32 | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| column | Int32 | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseFieldIndex | Int32 | L'index du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout de la Timeline

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Ajouter un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter le contrôle timeline
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| destCellName | String | Le nom de la cellule dans le coin supérieur gauche de la plage Timeline. |
| baseFieldIndex | Int32 | L'index du PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout de la Timeline

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualiser les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Trouver l'index du champ de base pour le champ "Date"
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // Ajouter la timeline en utilisant l'index trouvé
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // Enregistrer le résultat
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| ligne | Int32 | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| column | Int32 | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de la chronologie. |
| baseField | PivotField | Le PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout de la Timeline

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // Ajouter des champs pivot
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // Ajouter la timeline en utilisant le tableau croisé dynamique
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // Enregistrez le classeur
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | Objet PivotTable |
| destCellName | String | Le nom de la cellule dans le coin supérieur gauche de la plage Timeline. |
| baseField | PivotField | Le PivotField dans PivotTable.BaseFields |

### Valeur de retour

Le nouvel indice d'ajout de la Timeline

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ajouter la timeline en utilisant le tableau croisé dynamique comme source de données
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


