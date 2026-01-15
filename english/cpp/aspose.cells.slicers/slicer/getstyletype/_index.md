---
title: Aspose::Cells::Slicers::Slicer::GetStyleType method
linktitle: GetStyleType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Slicers::Slicer::GetStyleType method. Specify the type of Built-in slicer style. The default type is SlicerStyleLight1 in C++.'
type: docs
weight: 3500
url: /cpp/aspose.cells.slicers/slicer/getstyletype/
---
## Slicer::GetStyleType method


Specify the type of Built-in slicer style. The default type is SlicerStyleLight1.

```cpp
SlicerStyleType Aspose::Cells::Slicers::Slicer::GetStyleType()
```


## Examples


```cpp
if (slicer.GetStyleType() != SlicerStyleType::SlicerStyleLight2)
{
    slicer.SetStyleType(SlicerStyleType::SlicerStyleLight2);
}
```

## See Also

* Enum [SlicerStyleType](../../slicerstyletype/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
