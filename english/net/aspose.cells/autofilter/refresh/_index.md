---
title: AutoFilter.Refresh
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Refresh auto filters to hide or unhide the rows
type: docs
url: /net/aspose.cells/autofilter/refresh/
---
## Refresh() {#refresh}

Refresh auto filters to hide or unhide the rows.

```csharp
public int[] Refresh()
```

### Return Value

Returns all hidden rows' indexes.

### Examples

```csharp
// Called: autofilter1.Refresh();
[Test]
        public void Method_Refresh()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "AutoFilter/N22617.xls");

            Worksheet sheet = wb.Worksheets[0];
            AutoFilter autofilter1 = sheet.AutoFilter;

            autofilter1.Range = "A1:B1";
            autofilter1.Filter(0, "A");
            autofilter1.Refresh();
            sheet.Cells.HideRow(1);
            wb.Save(Constants.destPath +"filteredBook2.xls");
            wb = new Workbook(Constants.destPath + "filteredBook2.xls");
            Assert.AreEqual(0.0, wb.Worksheets[0].Cells.GetRowHeight(1));
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Refresh(bool) {#refresh_1}

Gets all hidden rows' indexes.

```csharp
public int[] Refresh(bool hideRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| hideRows | Boolean | If true, hide the filtered rows. |

### Return Value

Returns all hidden rows indexes.

### Examples

```csharp
// Called: int[] ret = wb.Worksheets[0].AutoFilter.Refresh(false);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46007.xlsx");
            int[] ret = wb.Worksheets[0].AutoFilter.Refresh(false);
            Assert.AreEqual(ret.Length, 1);
            Assert.AreEqual(ret[0], 1);
            ret = wb.Worksheets[0].AutoFilter.Refresh(true);
            Assert.AreEqual(ret.Length, 1);
            Assert.AreEqual(ret[0], 1);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);//.Save(Constants.destPath + "Cellsnet46007.xlsx");
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


