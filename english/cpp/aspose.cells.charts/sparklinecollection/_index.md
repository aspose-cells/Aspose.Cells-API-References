---
title: Aspose::Cells::Charts::SparklineCollection class
linktitle: SparklineCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SparklineCollection class. Encapsulates a collection of Sparkline objects in C++.'
type: docs
weight: 2900
url: /cpp/aspose.cells.charts/sparklinecollection/
---
## SparklineCollection class


Encapsulates a collection of [Sparkline](../sparkline/) objects.

```cpp
class SparklineCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const U16String\& dataRange, int32_t row, int32_t column)](./add/) | Add a sparkline. |
| [Add(const char16_t* dataRange, int32_t row, int32_t column)](./add/) | Add a sparkline. |
| [Get(int32_t index)](./get/) | Gets the [Sparkline](../sparkline/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SparklineCollection\& src)](./operator_asm/) | operator= |
| [Remove(const Aspose::Cells::Object\& o)](./remove/) |  **(Deprecated)** Removes the sparkline. |
| [RemoveSparkline(const Sparkline\& o)](./removesparkline/) | Removes the sparkline. |
| [SparklineCollection(SparklineCollection_Impl* impl)](./sparklinecollection/) | Constructs from an implementation object. |
| [SparklineCollection(const SparklineCollection\& src)](./sparklinecollection/) | Copy constructor. |
| [~SparklineCollection()](./~sparklinecollection/) | Destructor. |
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

int idx = sheet.GetSparklineGroups().Add(SparklineType::Line, sheet.GetName() + u"!A1:D1", false, ca);
SparklineGroup group = sheet.GetSparklineGroups().Get(idx);
group.GetSparklines().Add(sheet.GetName() + u"!A1:D1", 0, 4);
book.Save(u"output.xlsx", SaveFormat::Xlsx);
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
