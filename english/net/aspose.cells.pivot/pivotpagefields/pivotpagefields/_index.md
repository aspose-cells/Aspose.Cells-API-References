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
            Workbook workbook = new Workbook(Constants.openPivottablePath + &quot;PivotSource.xls&quot;);

            Worksheet ws = workbook.Worksheets[0];
            PivotTableCollection pivottables = ws.PivotTables;
            string[] src = { &quot;=Sheet1!A1:C8&quot;, &quot;=Sheet2!A1:C8&quot; };
            PivotPageFields page = new PivotPageFields();
            string[] items = new string[2];
            items[0] = &quot;item1&quot;;
            items[1] = &quot;item2&quot;;
            page.AddPageField(items);

            items = new string[2];
            items[0] = &quot;item3&quot;;
            items[1] = &quot;item4&quot;;
            page.AddPageField(items);

            int[] tb = new int[2];
            tb[0] = 0;
            tb[1] = 1;

            page.AddIdentify(0, tb);

            tb = new int[2];
            tb[0] = 1;
            tb[1] = -1;
            page.AddIdentify(1, tb);

            int index = pivottables.Add(src, false, page, &quot;E3&quot;, &quot;PivotTable1&quot;);


            //workbook.Save(&quot;D:\\c.xls&quot;, FileFormatType.Excel97To2003);
            workbook.Save(Constants.savePivottablePath + &quot;c.xlsx&quot;);


        }
```

### See Also

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


