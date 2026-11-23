---
title: "Protection.AllowUsingPivotTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowUsingPivotTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Activer la protection de la feuille
            Protection protection = worksheet.Protection;
            protection.AllowUsingPivotTable = true;
            worksheet.Protect(ProtectionType.All);

            // Vérifiez le paramètre
            Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);

            // Créer un tableau croisé dynamique pour démontrer la fonctionnalité
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Créer un tableau croisé dynamique avec les paramètres corrects
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Enregistrez le classeur
            workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


