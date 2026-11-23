---
title: "PivotTableCollection.Remove"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTableCollection méthode. Supprime le PivotTable spécifié et supprime les données du PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

Supprime le PivotTable spécifié et supprime les données du PivotTable

```csharp
public void Remove(PivotTable pivotTable)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Objet PivotTable |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtenir la collection de tableaux croisés dynamiques
            PivotTableCollection pivotTables = sheet.PivotTables;
            
            // Vérifier s'il existe des tableaux croisés dynamiques
            if (pivotTables.Count > 0)
            {
                // Obtenir le premier tableau croisé dynamique
                PivotTable pivotTable = pivotTables[0];
                
                // Supprimer le tableau croisé dynamique
                pivotTables.Remove(pivotTable);
                
                Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotTableRemoved.xlsx");
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

## Remove(PivotTable, bool) {#remove_1}

Supprime le PivotTable spécifié

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Objet PivotTable |
| keepData | Boolean | Indique s'il faut conserver les données du tableau croisé dynamique |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Démontrer la méthode Remove avec PivotTable et des paramètres booléens
            Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
            
            // Supprimer le tableau croisé dynamique mais conserver les données (true)
            worksheet.PivotTables.Remove(pivotTable, true);
            Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);

            // Ajouter un autre tableau croisé dynamique
            index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
            
            // Supprimer le tableau croisé dynamique et effacer les données (false)
            worksheet.PivotTables.Remove(pivotTable, false);
            Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


