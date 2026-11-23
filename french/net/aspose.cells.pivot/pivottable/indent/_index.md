---
title: "PivotTable.Indent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Spécifie l'incrément d'indentation pour l'axe compact et peut être utilisée pour définir la disposition du rapport en forme compacte"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

Spécifie l'incrément d'indentation pour l'axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte.

```csharp
public int Indent { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIndentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Définir la propriété d'indentation
            pivotTable.Indent = 3;
            Console.WriteLine("Pivot Table Indent: " + pivotTable.Indent);

            // Enregistrez le classeur
            workbook.Save("PivotTableIndentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


