---
title: "PivotPageFields.AddIdentify"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotPageFields. Définit quelle étiquette d'élément dans chaque champ de page utiliser pour identifier la plage de données. La propriété pageItemIndex.Length doit être égale à PageFieldCount, veuillez donc ajouter le champ de page en premier."
type: docs
url: /fr/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Définit quelle étiquette d'élément dans chaque champ de page utiliser pour identifier la plage de données. La longueur de pageItemIndex doit être égale à PageFieldCount, veuillez donc ajouter d'abord le champ de page.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rangeIndex | Int32 | L'index de la plage de données de consolidation. |
| pageItemIndex | Int32[] | L'index de l'élément de page dans chaque champ de page. pageItemIndex[2] = 1 signifie que le deuxième élément du troisième champ est utilisé pour identifier cette plage. pageItemIndex[1] = -1 signifie qu'aucun élément du deuxième champ n'est utilisé pour identifier cette plage et que MS créera automatiquement un élément "blank" dans le deuxième champ pour identifier cette plage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Instancier PivotPageFields directement au lieu d'y accéder via PivotTable
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


