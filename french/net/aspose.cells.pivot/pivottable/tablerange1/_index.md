---
title: "PivotTable.TableRange1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTable property. Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport PivotTable mais n'inclut pas les champs de page. Lecture seule"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/tablerange1/
---
## PivotTable.TableRange1 property

Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport PivotTable, mais n'inclut pas les champs de page. Lecture seule.

```csharp
public CellArea TableRange1 { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange1Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul avec des données d'exemple
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Créer un tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            int pivotTableIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            int labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Configurer le tableau croisé dynamique
            pivotTable.ShowInTabularForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Démontrer la propriété TableRange1
            Console.WriteLine("Pivot Table Range:");
            Console.WriteLine($"Start Row: {pivotTable.TableRange1.StartRow}");
            Console.WriteLine($"End Row: {pivotTable.TableRange1.EndRow}");
            Console.WriteLine($"Start Column: {pivotTable.TableRange1.StartColumn}");
            Console.WriteLine($"End Column: {pivotTable.TableRange1.EndColumn}");

            // Enregistrez le classeur
            workbook.Save("PivotTablePropertyTableRange1Demo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


