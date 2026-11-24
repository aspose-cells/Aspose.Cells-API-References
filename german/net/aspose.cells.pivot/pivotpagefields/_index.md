---
title: "Klasse PivotPageFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotPageFields Klasse. Stellt die Pivot-Seitenobjekte dar, wenn die Datenquelle der Pivot-Tabelle Konsolidierungsbereiche sind. Sie kann nur bis zu 4 Elemente enthalten."
type: docs
url: /de/net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Stellt die Pivot‑Seitenobjekte dar, wenn die Datenquelle der Pivot‑Tabelle Konsolidierungsbereiche ist. Sie kann höchstens 4 Elemente enthalten.

```csharp
public class PivotPageFields
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | Stellt die Pivot-Seitenfeld-Elemente dar. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | Liefert die Anzahl der Seitenfelder. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | Legt fest, welches Elementlabel in jedem Seitenfeld verwendet wird, um den Datenbereich zu identifizieren. Die pageItemIndex.Length muss gleich PageFieldCount sein, daher fügen Sie bitte zuerst das Seitenfeld hinzu. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | Fügt ein Seitenfeld hinzu. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


