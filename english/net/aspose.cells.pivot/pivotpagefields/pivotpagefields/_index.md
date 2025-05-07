---
title: PivotPageFields.PivotPageFields
second_title: Aspose.Cells for .NET API Reference
description: PivotPageFields constructor. Represents the pivot page field items
type: docs
url: /net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Represents the pivot page field items.

```csharp
public PivotPageFields()
```

### Examples

```csharp
// Called: PivotPageFields page = new PivotPageFields();
[Test]
        public void PivotPageFields_Constructor()
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

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


