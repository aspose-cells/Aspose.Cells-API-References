---
title: "PivotPageFields.AddPageField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotPageFields. Ajoute un champ de page"
type: docs
url: /fr/net/aspose.cells.pivot/pivotpagefields/addpagefield/
---
## PivotPageFields.AddPageField method

Ajoute un champ de page.

```csharp
public void AddPageField(string[] pageItems)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageItems | String[] | Étiquette d'élément du champ de page |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddPageFieldWithStringArrayDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            string[] consolidationRanges = { "A1:B3" };
            PivotPageFields pageFields = new PivotPageFields();
            int pivotIndex = worksheet.PivotTables.Add(
                consolidationRanges,
                false,
                pageFields,
                "D1",
                "MyPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            try
            {
                pageFields.AddPageField(new string[] { "North", "South" });
                Console.WriteLine("AddPageField executed successfully with parameters (String[])");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("AddPageFieldStringArrayDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


