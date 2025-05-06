---
title: LoadFilter.LoadFilter
second_title: Aspose.Cells for .NET API Reference
description: LoadFilter constructor. Constructs one LoadFilter with default filter options LoadDataFilterOptions.All
type: docs
url: /net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Constructs one LoadFilter with default filter options LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Examples

```csharp
// Called: LoadFilter filter = new LoadFilter();
private void LoadFilter_Constructor(string path, int limit)
        {
            LoadFilter filter = new LoadFilter();
            InterrupHandler handler = new InterrupHandler(limit, filter);
            Workbook wb = new Workbook(path,
                new LoadOptions() { LoadFilter = filter, LightCellsDataHandler = handler });
            Assert.IsTrue(handler.Exceeded, &quot;Dataset&apos;s size should exceed the limit&quot;);
            int count = 0;
            foreach (Worksheet sheet in wb.Worksheets)
            {
                count += sheet.Cells.Count;
            }
            Assert.AreEqual(count, limit, path + &quot;: the cell count&quot;);
        }
```

### See Also

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Constructs one LoadFilter with given filter options.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| opts | LoadDataFilterOptions | the default filter options |

### See Also

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


