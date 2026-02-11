---
title: Aspose::Cells::Charts::SparklineGroupCollection class
linktitle: SparklineGroupCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SparklineGroupCollection class. Encapsulates a collection of SparklineGroup objects in C++.'
type: docs
weight: 3100
url: /cpp/aspose.cells.charts/sparklinegroupcollection/
---
## SparklineGroupCollection class


Encapsulates a collection of [SparklineGroup](../sparklinegroup/) objects.

```cpp
class SparklineGroupCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(SparklineType type)](./add/) | Adds an [SparklineGroup](../sparklinegroup/) with a [Sparkline](../sparkline/) to the collection. |
| [Add(SparklineType type, const U16String\& dataRange, bool isVertical, const CellArea\& locationRange)](./add/) | Adds an [SparklineGroup](../sparklinegroup/) with some [Sparkline](../sparkline/) to the collection. |
| [Add(SparklineType type, const char16_t* dataRange, bool isVertical, const CellArea\& locationRange)](./add/) | Adds an [SparklineGroup](../sparklinegroup/) with some [Sparkline](../sparkline/) to the collection. |
| [ClearSparklineGroups(const CellArea\& cellArea)](./clearsparklinegroups/) | Clears the sparkline groups that overlaps an area of cells. |
| [ClearSparklines(const CellArea\& cellArea)](./clearsparklines/) | Clears the sparklines that is inside an area of cells. |
| [Get(int32_t index)](./get/) | Gets the [SparklineGroup](../sparklinegroup/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SparklineGroupCollection\& src)](./operator_asm/) | operator= |
| [SparklineGroupCollection(SparklineGroupCollection_Impl* impl)](./sparklinegroupcollection/) | Constructs from an implementation object. |
| [SparklineGroupCollection(const SparklineGroupCollection\& src)](./sparklinegroupcollection/) | Copy constructor. |
| [~SparklineGroupCollection()](./~sparklinegroupcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);

sheet.GetCells().Get(u"A1").PutValue(5);
sheet.GetCells().Get(u"B1").PutValue(2);
sheet.GetCells().Get(u"C1").PutValue(1);
sheet.GetCells().Get(u"D1").PutValue(3);

// Define the CellArea
CellArea ca;
ca.StartColumn = 4;
ca.EndColumn = 4;
ca.StartRow = 0;
ca.EndRow = 0;

int idx = sheet.GetSparklineGroups().Add(SparklineType::Line, u"A1:D1", false, ca);
SparklineGroup group = sheet.GetSparklineGroups().Get(idx);
group.GetSparklines().Add(sheet.GetName() + u"!A1:D1", 0, 4);
book.Save(u"output.xlsx", SaveFormat::Xlsx);
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
