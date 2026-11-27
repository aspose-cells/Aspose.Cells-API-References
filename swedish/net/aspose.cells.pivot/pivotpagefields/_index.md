---
title: "Klass PivotPageFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotPageFields-klass. Representerar pivot-sidobjekt om pivottabellens datakälla är konsolideringsområden. Den kan bara innehålla upp till 4 objekt."
type: docs
url: /sv/net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Representerar pivotsidobjekten om pivottabellens datakälla är konsolideringsområden. Den kan bara innehålla upp till 4 objekt.

```csharp
public class PivotPageFields
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | Representerar pivot-sidfältsobjekten. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | Hämtar antalet sidfält. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | Anger vilken objektetikett i varje sidfält som ska användas för att identifiera dataintervallet. pageItemIndex.Length måste vara lika med PageFieldCount, så lägg till sidfältet först. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | Lägger till ett sidfält. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


