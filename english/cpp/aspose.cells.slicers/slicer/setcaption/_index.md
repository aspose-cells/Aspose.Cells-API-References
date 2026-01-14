---
title: Aspose::Cells::Slicers::Slicer::SetCaption method
linktitle: SetCaption
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Slicers::Slicer::SetCaption method. Returns or sets the caption of the specified slicer in C++.'
type: docs
weight: 4000
url: /cpp/aspose.cells.slicers/slicer/setcaption/
---
## Slicer::SetCaption(const U16String\&) method


Returns or sets the caption of the specified slicer.

```cpp
void Aspose::Cells::Slicers::Slicer::SetCaption(const U16String &value)
```


## Examples


```cpp
U16String val = u"slicer caption";
if (slicer.GetCaption().IsNull())
{
    slicer.SetCaption(val);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## Slicer::SetCaption(const char16_t*) method


Returns or sets the caption of the specified slicer.

```cpp
void Aspose::Cells::Slicers::Slicer::SetCaption(const char16_t *value)
```


## Examples


```cpp
if(slicer.GetCaption().IsNull())
{
    slicer.SetCaption(u"slicer caption");
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
