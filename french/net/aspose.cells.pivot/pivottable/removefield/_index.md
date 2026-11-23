---
title: "PivotTable.RemoveField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Supprime un champ d'une zone de champ spécifique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Supprime un champ d'une zone de champ spécifique

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | Le type de zone des champs. |
| fieldName | String | Le nom dans les champs de base. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Supprimer le champ "c" de la zone Données
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // Calculer les données du tableau croisé dynamique
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Supprime un champ d'une région pivot spécifique.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | Le type de zone des champs. |
| baseFieldIndex | Int32 | L'index du champ dans les champs de base. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Supprimer le champ de ligne (indice 0) du tableau croisé dynamique
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Supprime le champ d'une zone de champ spécifique

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | le type de zone des champs. |
| pivotField | PivotField | le champ dans les champs de base. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Supprimer un champ de colonne du tableau croisé dynamique
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // Supprimer un champ de données du tableau croisé dynamique
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // Enregistrez le classeur
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


