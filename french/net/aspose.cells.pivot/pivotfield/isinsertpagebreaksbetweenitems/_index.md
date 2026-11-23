---
title: "PivotField.IsInsertPageBreaksBetweenItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique s'il faut insérer des sauts de page après chaque élément. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/
---
## PivotField.IsInsertPageBreaksBetweenItems property

Indique s'il faut insérer des sauts de page après chaque élément. La valeur par défaut est fausse.

```csharp
public bool IsInsertPageBreaksBetweenItems { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsInsertPageBreaksBetweenItemsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 7; i++)
            {
                worksheet.Cells["A" + i].PutValue("Category " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Vérifier le nombre de pages avant de définir la propriété
            SheetRender render1 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count before: " + render1.PageCount);

            // Définir la propriété IsInsertPageBreaksBetweenItems
            PivotField field = pivotTable.RowFields[0];
            field.IsInsertPageBreaksBetweenItems = true;
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Vérifier le nombre de pages après avoir défini la propriété
            SheetRender render2 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count after: " + render2.PageCount);

            // Enregistrez le classeur
            workbook.Save("PivotFieldIsInsertPageBreaksBetweenItemsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


