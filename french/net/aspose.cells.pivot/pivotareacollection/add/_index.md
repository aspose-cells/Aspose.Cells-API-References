---
title: "PivotAreaCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotAreaCollection. Ajoute une zone pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotareacollection/add/
---
## Add(PivotArea) {#add}

Ajoute une zone pivot.

```csharp
[Obsolete("Use PivotAreaCollection.AddPivotArea(PivotArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(PivotArea pivotArea)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivotArea | PivotArea | La zone pivot. |

### Remarques

REMARQUE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode AddPivotArea(). Cette méthode sera supprimée 6 mois plus tard à partir de décembre 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionMethodAddWithPivotAreaDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("PivotTable");
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un tableau croisé dynamique
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Ajoutez des champs aux zones du tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Créer un format conditionnel
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            // Créez une zone pivot et ajoutez-la à la collection
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            pcf.PivotAreas.Add(pivotArea);

            // Ajoutez une condition de format
            FormatCondition fc = pcf.FormatConditions[pcf.FormatConditions.AddCondition(FormatConditionType.CellValue)];
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Formula1 = "15";
            fc.Style.BackgroundColor = Color.Yellow;

            // Calculez les données et enregistrez
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotAreaCollectionMethodAddWithPivotAreaDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Ajoute une zone basée sur la vue du tableau croisé dynamique.

```csharp
public void Add(CellArea cellArea)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | La zone basée sur la vue du tableau pivot. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Définir une zone de cellules à ajouter aux zones de tableau croisé dynamique
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 0;
            cellArea.StartColumn = 0;
            cellArea.EndRow = 2;
            cellArea.EndColumn = 1;

            // Obtenir la collection de zones de pivot en sélectionnant la zone
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea);

            try
            {
                // Appeler la méthode Add avec le paramètre CellArea
                pivotAreas.Add(cellArea);

                Console.WriteLine("Pivot area added successfully for cell area: " +
                    $"({cellArea.StartRow},{cellArea.StartColumn}) to ({cellArea.EndRow},{cellArea.EndColumn})");

                // Afficher les zones de pivot ajoutées
                foreach (PivotArea area in pivotAreas)
                {
                    CellArea[] areas = area.GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Pivot area covers: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("PivotAreaCollectionMethodAddWithCellAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


