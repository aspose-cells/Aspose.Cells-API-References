---
title: Workbook.StartAccessCache
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Starts the session that uses caches to access data
type: docs
url: /net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Starts the session that uses caches to access data.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |

### Remarks

If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them.  After finishing the access to the data, [`CloseAccessCache`](../closeaccesscache/) should be invoked with same options to clear all caches and recover normal access mode.

### Examples

```csharp
// Called: wb.StartAccessCache(AccessCacheOptions.All);
public void Workbook_Method_StartAccessCache()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
    cfc[cfc.Add()].Add(CellArea.CreateCellArea(0, 0, 5, 0),
        FormatConditionType.DuplicateValues, OperatorType.None, null, null);
    Style style = cfc[0][0].Style;
    style.ForegroundColor = Color.Red;
    style.Pattern = BackgroundType.Solid;
    Cells cells = sheet.Cells;
    byte[] img = File.ReadAllBytes(Constants.sourcePath + "1.png");
    cells[0, 0].EmbeddedImage = img;
    cells[2, 0].EmbeddedImage = File.ReadAllBytes(Constants.sourcePath + "2.png");
    cells[4, 0].EmbeddedImage = img;

    Assert.AreEqual(BackgroundType.Solid, cells[0, 0].GetDisplayStyle().Pattern, "A1");
    Assert.AreEqual(BackgroundType.None, cells[2, 0].GetDisplayStyle().Pattern, "A3");
    Assert.AreEqual(BackgroundType.Solid, cells[4, 0].GetDisplayStyle().Pattern, "A5");

    wb.StartAccessCache(AccessCacheOptions.All);
    Assert.AreEqual(BackgroundType.Solid, cells[0, 0].GetDisplayStyle().Pattern, "A1");
    Assert.AreEqual(BackgroundType.None, cells[2, 0].GetDisplayStyle().Pattern, "A3");
    Assert.AreEqual(BackgroundType.Solid, cells[4, 0].GetDisplayStyle().Pattern, "A5");
    wb.CloseAccessCache(AccessCacheOptions.All);
}
```

### See Also

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


