---
title: "PivotTableCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTableCollection propriété. Obtient le rapport PivotTable par index"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Obtient le rapport PivotTable par index.

```csharp
public PivotTable this[int index] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de tableaux croisés dynamiques
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Accéder au premier tableau croisé dynamique en utilisant la propriété Item (indexeur)
            PivotTable pivotTable = pivotTables[0];
            
            // Calculer les données du tableau croisé dynamique
            pivotTable.CalculateData();
            
            // Enregistrer le classeur modifié
            workbook.Save("output.xlsx");
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

## PivotTableCollection indexer (2 of 3)

Obtient le rapport PivotTable par le nom du PivotTable.

```csharp
public PivotTable this[string name] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(3000);

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configurer le tableau croisé dynamique en utilisant la propriété Item
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualiser et calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Accéder au tableau croisé dynamique en utilisant la propriété Item
            PivotTable tableFromCollection = sheet.PivotTables["PivotTable1"];
            Console.WriteLine("Pivot table data source: " + string.Join(", ", tableFromCollection.DataSource));

            // Modifier les données et actualiser
            sheet.Cells["B2"].PutValue(1500);
            tableFromCollection.RefreshData();
            Console.WriteLine("Updated pivot table values");

            // Enregistrez le classeur
            workbook.Save("PivotTableDemo.xlsx");
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

## PivotTableCollection indexer (3 of 3)

Obtient le [`PivotTable`](../../pivottable/) situé dans la cellule.

```csharp
public PivotTable this[int row, int column] { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 3000;

            try
            {
                // Ajoutez un tableau croisé dynamique à la feuille de calcul
                int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");

                // Accéder à la PivotTableCollection
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Démontrer l'accès à un tableau croisé dynamique en utilisant la propriété Item (indexeur)
                PivotTable pivotTable = pivotTables[index];
                Console.WriteLine($"Accessed pivot table at index {index} with name: {pivotTable.Name}");

                // Démontrer l'accès par nom en utilisant la propriété Item
                PivotTable pivotTableByName = pivotTables["PivotTable1"];
                Console.WriteLine($"Accessed pivot table by name: {pivotTableByName.Name}");

                // Configurer le tableau croisé dynamique
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Actualiser et calculer les données
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Enregistrez le classeur
                workbook.Save("PivotTableItemDemo.xlsx");
                Console.WriteLine("Pivot table demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
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


