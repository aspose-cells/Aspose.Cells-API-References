---
title: Aspose::Cells::Slicers::Slicer::SetName method
linktitle: SetName
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Slicers::Slicer::SetName method. Returns or sets the name of the specified slicer in C++.'
type: docs
weight: 3800
url: /cpp/aspose.cells.slicers/slicer/setname/
---
## Slicer::SetName(const U16String\&) method


Returns or sets the name of the specified slicer.

```cpp
void Aspose::Cells::Slicers::Slicer::SetName(const U16String &value)
```


## Examples


```cpp
U16String val = u"slicer name";
if (slicer.GetName().IsNull())
{
    slicer.SetName(val);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## Slicer::SetName(const char16_t*) method


Returns or sets the name of the specified slicer.

```cpp
void Aspose::Cells::Slicers::Slicer::SetName(const char16_t *value)
```


## Examples


```cpp
if (slicer.GetName().IsNull())
{
    slicer.SetName(u"slicer name");
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
