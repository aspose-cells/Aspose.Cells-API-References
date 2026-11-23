---
title: "PivotTableCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTableCollection. Supprime le tableau croisé dynamique à l'index spécifié et supprime les données du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablecollection/removeat/
---
## RemoveAt(int) {#removeat}

Supprime le tableau croisé dynamique à l'index spécifié et supprime les données du tableau croisé dynamique

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | l'index de position dans la collection de tableaux croisés dynamiques |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Ajouter plusieurs tableaux croisés dynamiques
            sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            sheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            sheet.PivotTables.Add("A1:B4", "D20", "PivotTable3");

            // Supprimer le tableau croisé dynamique à l'index 1 (deuxième tableau croisé dynamique)
            sheet.PivotTables.RemoveAt(1);

            // Vérifier le nombre après la suppression
            Console.WriteLine("Pivot Tables Count: " + sheet.PivotTables.Count);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_2}

Supprime la PivotTable à l'index spécifié

```csharp
public void RemoveAt(int index, bool keepData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | l'index de position dans la collection de tableaux croisés dynamiques |
| keepData | Boolean | Indique s'il faut conserver les données du tableau croisé dynamique |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Démontrer RemoveAt avec keepData=true
            worksheet.PivotTables.RemoveAt(0, true);
            Console.WriteLine("Pivot table removed with keepData=true. Cell D9 value: " + worksheet.Cells["D9"].Value);

            // Ajouter un autre tableau croisé dynamique
            index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Démontrer RemoveAt avec keepData=false
            worksheet.PivotTables.RemoveAt(0, false);
            Console.WriteLine("Pivot table removed with keepData=false. Cell D9 value: " + worksheet.Cells["D9"].Value);
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


