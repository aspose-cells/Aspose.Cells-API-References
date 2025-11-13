---
title: Class PivotPageFields
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotPageFields class. Represents the pivot page items if the pivot table data source is consolidation ranges. It only can contain up to 4 items
type: docs
url: /net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Represents the pivot page items if the pivot table data source is consolidation ranges. It only can contain up to 4 items.

```csharp
public class PivotPageFields
```

## Constructors

| Name | Description |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | Represents the pivot page field items. |

## Properties

| Name | Description |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | Gets the number of page fields. |

## Methods

| Name | Description |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | Adds a page field. |

### Examples

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

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


