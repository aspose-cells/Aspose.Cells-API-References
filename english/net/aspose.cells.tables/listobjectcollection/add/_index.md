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
// Called: tables.Add(1, 0, 5, 2, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ListObjectCollection tables = sheet.ListObjects;
            tables.Add(1, 0, 5, 2, true);
            wb.Replace("Column1", "Column2");

            Util.SetHintMessage(sheet.Cells[0, 0], "This file should not cause corrupted message when opened by ms excel");
            //Util.SaveManCheck(wb, "", "J43231.xlsx");
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
// Called: listObjects.Add("A1", "B4", true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("a");
            cells[1, 0].PutValue(1);
            cells[2, 0].PutValue(2);
            cells[3, 0].PutValue(3);
            cells[0, 1].PutValue("b");
            cells[1, 1].PutValue(4);
            cells[2, 1].PutValue(5);
            cells[3, 1].PutValue(6);

            ListObjectCollection listObjects = workbook.Worksheets[0].ListObjects;
            listObjects.Add("A1", "B4", true);
            listObjects[0].ShowTotals = true;
            workbook.Save(Constants.destPath + "testListObject.xlsx", SaveFormat.Xlsx);

            workbook = new Workbook(Constants.destPath + "testListObject.xlsx");
            listObjects = workbook.Worksheets[0].ListObjects;
            AssertHelper.AreEqual(true, listObjects[0].ShowTotals, "listObjects[0].ShowTotals");
            //workbook.Worksheets.TableStyles.AddTableStyle(
            //listObjects[0].TableStyleType 
        }
```

### See Also

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


