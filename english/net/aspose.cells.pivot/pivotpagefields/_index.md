---
title: Class PivotPageFields
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotPageFields class. Represents the pivot page field items if the pivot table data source is consolidation ranges. It only can contain up to 4 fields
type: docs
url: /net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Represents the pivot page field items if the pivot table data source is consolidation ranges. It only can contain up to 4 fields.

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
// Called: PivotPageFields page = new PivotPageFields();
[Test]
        public void Type_PivotPageFields()
        {
            Workbook workbook = new Workbook(Constants.openPivottablePath + "PivotSource.xls");

            Worksheet ws = workbook.Worksheets[0];
            PivotTableCollection pivottables = ws.PivotTables;
            string[] src = { "=Sheet1!A1:C8", "=Sheet2!A1:C8" };
            PivotPageFields page = new PivotPageFields();
            string[] items = new string[2];
            items[0] = "item1";
            items[1] = "item2";
            page.AddPageField(items);

            items = new string[2];
            items[0] = "item3";
            items[1] = "item4";
            page.AddPageField(items);

            int[] tb = new int[2];
            tb[0] = 0;
            tb[1] = 1;

            page.AddIdentify(0, tb);

            tb = new int[2];
            tb[0] = 1;
            tb[1] = -1;
            page.AddIdentify(1, tb);

            int index = pivottables.Add(src, false, page, "E3", "PivotTable1");


            //workbook.Save("D:\\c.xls", FileFormatType.Excel97To2003);
            workbook.Save(Constants.savePivottablePath + "c.xlsx");


        }
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


