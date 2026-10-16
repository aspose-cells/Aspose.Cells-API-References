---
title: Aspose::Cells::Pivot::PivotFieldGroupOptions::SetGroupType method
linktitle: SetGroupType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFieldGroupOptions::SetGroupType method. Gets or sets the grouping type for pivot field. Only for grouping date time pivot field in C++.'
type: docs
weight: 2100
url: /cpp/aspose.cells.pivot/pivotfieldgroupoptions/setgrouptype/
---
## PivotFieldGroupOptions::SetGroupType method


Gets or sets the grouping type for pivot field. Only for grouping date time pivot field.

```cpp
void Aspose::Cells::Pivot::PivotFieldGroupOptions::SetGroupType(PivotGroupByType value)
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

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotGroupByType](../../pivotgroupbytype/)
* Class [PivotFieldGroupOptions](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
