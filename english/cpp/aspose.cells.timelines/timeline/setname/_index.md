---
title: Aspose::Cells::Timelines::Timeline::SetName method
linktitle: SetName
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Timelines::Timeline::SetName method. Returns or sets the name of the specified Timeline in C++.'
type: docs
weight: 2400
url: /cpp/aspose.cells.timelines/timeline/setname/
---
## Timeline::SetName(const U16String\&) method


Returns or sets the name of the specified [Timeline](../).

```cpp
void Aspose::Cells::Timelines::Timeline::SetName(const U16String &value)
```


## Examples


```cpp
//Set the name of the specified Timeline.
if (timelineObj.GetName().IsNull())
{
    U16String val = u"timeline name test";
    timelineObj.SetName(val);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Timeline](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## Timeline::SetName(const char16_t*) method


Returns or sets the name of the specified [Timeline](../).

```cpp
void Aspose::Cells::Timelines::Timeline::SetName(const char16_t *value)
```


## Examples


```cpp
//Set the name of the specified Timeline.
if (timelineObj.GetName().IsNull())
{
    timelineObj.SetName(u"timeline name test");
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Timeline](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
