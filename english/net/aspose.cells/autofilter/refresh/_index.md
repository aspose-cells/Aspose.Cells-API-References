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
// Called: worksheet.AutoFilter.Refresh();
public void AutoFilter_Method_Refresh()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.AutoFilter.Range = "B6:K6";
    worksheet.AutoFilter.Custom(4, FilterOperatorType.GreaterThan, 500);
    worksheet.AutoFilter.Refresh();
    Assert.IsTrue(worksheet.Cells.IsRowHidden(7));
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    worksheet = workbook.Worksheets[0];
    worksheet.AutoFilter.Range = "B6:K6";
    worksheet.AutoFilter.Custom(5, FilterOperatorType.Equal, "", false, FilterOperatorType.GreaterThan, 500); 
    worksheet.AutoFilter.Refresh();
    Assert.IsFalse(worksheet.Cells.IsRowHidden(13));
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    worksheet = workbook.Worksheets[0];
    worksheet.AutoFilter.Range = "B6:K6";
    worksheet.AutoFilter.FilterTop10(5, false, false, 5); 
    worksheet.AutoFilter.Refresh();
    Assert.IsTrue(worksheet.Cells.IsRowHidden(13));
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    worksheet = workbook.Worksheets[0];
    worksheet.AutoFilter.Range = "B6:K6";
    worksheet.AutoFilter.FilterTop10(5, true, false, 5);
    worksheet.AutoFilter.Refresh();
    Assert.IsTrue(worksheet.Cells.IsRowHidden(13));
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
// Called: int[] rows = wSheet.AutoFilter.Refresh(false);//It shows correct row numbers that are hidden due to filter
public void AutoFilter_Method_Refresh()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet wSheet = workbook.Worksheets[0];
    if (wSheet.HasAutofilter)
    {
        Console.WriteLine("Autofilter detected");
        int[] rows = wSheet.AutoFilter.Refresh(false);//It shows correct row numbers that are hidden due to filter
        wSheet.AutoFilter.ShowAll();
        int[] rows2 = wSheet.AutoFilter.Refresh(false);//It shows correct result as null
    }
    Assert.IsFalse(wSheet.Cells.IsRowHidden(13));
    Assert.IsFalse(wSheet.Cells.IsRowHidden(15));
    //.Save(Constants.destPath + "example.xlsx");//In the output file rows containing value 2 are missing
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


