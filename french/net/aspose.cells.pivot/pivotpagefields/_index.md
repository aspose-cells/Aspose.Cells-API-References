---
title: "Classe PivotPageFields"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotPageFields. Représente les éléments de page du tableau croisé dynamique si la source de données du tableau croisé dynamique est des plages de consolidation. Elle ne peut contenir que jusqu'à 4 éléments"
type: docs
url: /fr/net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Représente les éléments de page du tableau croisé dynamique si la source de données du tableau croisé dynamique est des plages de consolidation. Il ne peut contenir que jusqu'à 4 éléments.

```csharp
public class PivotPageFields
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | Représente les éléments de champ de page du tableau croisé dynamique. |

## Propriétés

| Nom | Description |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | Obtient le nombre de champs de page. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | Définit quelle étiquette d'élément dans chaque champ de page utiliser pour identifier la plage de données. La longueur de pageItemIndex doit être égale à PageFieldCount, veuillez donc ajouter d'abord le champ de page. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | Ajoute un champ de page. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotPageFieldsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Sheet1";
            FillData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            FillData(sheet2);

            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;

            string[] src = { "=Sheet1!A1:C8", "=Sheet2!A1:C8" };
            PivotPageFields pageFields = new PivotPageFields();

            pageFields.AddPageField(new string[] { "item1", "item2" });
            pageFields.AddPageField(new string[] { "item3", "item4" });

            pageFields.AddIdentify(0, new int[] { 0, 1 });
            pageFields.AddIdentify(1, new int[] { 1, -1 });

            pivotTables.Add(src, false, pageFields, "E3", "PivotTable1");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }

        private static void FillData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Value");
            cells["C1"].PutValue("Date");

            for (int i = 1; i < 8; i++)
            {
                cells[$"A{i+1}"].PutValue($"Item{i}");
                cells[$"B{i+1}"].PutValue(i * 100);
                cells[$"C{i+1}"].PutValue(System.DateTime.Now.AddDays(i).ToString("yyyy-MM-dd"));
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


