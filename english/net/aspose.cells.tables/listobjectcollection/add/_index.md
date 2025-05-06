---
title: ListObjectCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ListObjectCollection method. Adds a ListObject to the worksheet
type: docs
url: /net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Adds a ListObject to the worksheet.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row of the list range. |
| startColumn | Int32 | The start row of the list range. |
| endRow | Int32 | The start row of the list range. |
| endColumn | Int32 | The start row of the list range. |
| hasHeaders | Boolean | Whether the range has headers. |

### Return Value

The index of the new ListObject

### Examples

```csharp
// Called: ListObject listObject = sheet.ListObjects[sheet.ListObjects.Add(1, 0, 3, 1, true)];
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            Util.SetHintMessage(cells[0, 0], &quot;The file should not be corrupted or in protected view while loading by ms excel&quot;);

            cells[1, 0].PutValue(&quot;Column A&quot;);
            cells[1, 1].PutValue(&quot;Column B&quot;);
            cells[2, 0].PutValue(1);
            cells[2, 1].PutValue(3);

            ListObject listObject = sheet.ListObjects[sheet.ListObjects.Add(1, 0, 3, 1, true)];
            listObject.TableStyleType = TableStyleType.TableStyleMedium2;
            listObject.DisplayName = &quot;Table&quot;;
            //listObject.ListColumns[1].Formula = &quot;=[Column A] + 1&quot;;
            listObject.ShowTotals = true;
            listObject.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;
            Util.SaveManCheck(wb, &quot;Formula&quot;, &quot;N46991.xls&quot;);
            wb = new Workbook(Constants.checkPath + &quot;Formula/N46991.xls&quot;);
            Util.SaveManCheck(wb, &quot;Formula&quot;, &quot;N46991.xlsx&quot;);
        }
```

### See Also

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Adds a ListObject to the worksheet.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startCell | String | The start cell of the list range. |
| endCell | String | The end cell of the list range. |
| hasHeaders | Boolean | Whether the range has headers. |

### Return Value

The index of the new ListObject

### Examples

```csharp
// Called: listObjects.Add(&amp;quot;A1&amp;quot;, &amp;quot;B4&amp;quot;, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;a&quot;);
            cells[1, 0].PutValue(1);
            cells[2, 0].PutValue(2);
            cells[3, 0].PutValue(3);
            cells[0, 1].PutValue(&quot;b&quot;);
            cells[1, 1].PutValue(4);
            cells[2, 1].PutValue(5);
            cells[3, 1].PutValue(6);

            ListObjectCollection listObjects = workbook.Worksheets[0].ListObjects;
            listObjects.Add(&quot;A1&quot;, &quot;B4&quot;, true);
            workbook.Save(Constants.destPath + &quot;testListObject.xlsx&quot;, SaveFormat.Xlsx);

            workbook = new Workbook(Constants.destPath + &quot;testListObject.xlsx&quot;);
            listObjects = workbook.Worksheets[0].ListObjects;
            ListObject listObject = listObjects[0];
            AssertHelper.AreEqual(false, listObject.ShowTableStyleFirstColumn, &quot;listObject.ShowTableStyleFirstColumn&quot;);
        }
```

### See Also

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


