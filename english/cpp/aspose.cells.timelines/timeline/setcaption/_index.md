---
title: Aspose::Cells::Timelines::Timeline::SetCaption method
linktitle: SetCaption
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Timelines::Timeline::SetCaption method. Gets or sets the caption of this Timeline in C++.'
type: docs
weight: 2100
url: /cpp/aspose.cells.timelines/timeline/setcaption/
---
## Timeline::SetCaption(const U16String\&) method


Gets or sets the caption of this [Timeline](../).

```cpp
void Aspose::Cells::Timelines::Timeline::SetCaption(const U16String &value)
```


## Examples


```cpp
//Set the caption of the specified Timeline.
U16String val = u"timeline caption test";
if(timelineObj.GetCaption().IsNull())
{
    timelineObj.SetCaption(val);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Timeline](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## Timeline::SetCaption(const char16_t*) method


Gets or sets the caption of this [Timeline](../).

```cpp
void Aspose::Cells::Timelines::Timeline::SetCaption(const char16_t *value)
```


## Examples


```cpp
    //Set the caption of the specified Timeline.
if (timelineObj.GetCaption().IsNull())
{
    timelineObj.SetCaption(u"timeline caption test");
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Timeline](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
