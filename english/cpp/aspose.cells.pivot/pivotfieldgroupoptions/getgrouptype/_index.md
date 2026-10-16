---
title: Aspose::Cells::Pivot::PivotFieldGroupOptions::GetGroupType method
linktitle: GetGroupType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFieldGroupOptions::GetGroupType method. Gets or sets the grouping type for pivot field. Only for grouping date time pivot field in C++.'
type: docs
weight: 2000
url: /cpp/aspose.cells.pivot/pivotfieldgroupoptions/getgrouptype/
---
## PivotFieldGroupOptions::GetGroupType method


Gets or sets the grouping type for pivot field. Only for grouping date time pivot field.

```cpp
PivotGroupByType Aspose::Cells::Pivot::PivotFieldGroupOptions::GetGroupType()
```


## Examples


```cpp
Aspose::Cells::Startup();
// init
PivotFieldGroupOptions pivotFieldGroupOptions;
// Group by year and month together
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GetGroupType();
pivotGroupByType = PivotGroupByType::Years | PivotGroupByType::Months;
pivotFieldGroupOptions.SetGroupType(pivotGroupByType);
Aspose::Cells::Cleanup();
```

## See Also

* Enum [PivotGroupByType](../../pivotgroupbytype/)
* Class [PivotFieldGroupOptions](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
