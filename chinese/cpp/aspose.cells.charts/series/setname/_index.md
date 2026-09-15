---
title: Aspose::Cells::Charts::Series::SetName method
linktitle: SetName
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Series::SetName method. Gets or sets the name of the data series in C++.'
type: docs
weight: 1400
url: /zh/cpp/aspose.cells.charts/series/setname/
---
## Series::SetName(const U16String\&) method


Gets or sets the name of the data series.

```cpp
void Aspose::Cells::Charts::Series::SetName(const U16String &value)
```


## Examples


```cpp
//引用单元格的名称
U16String val = u"=A1";
chart.GetNSeries().Get(0).SetName(val);

//设置字符串为名称
val = u"First Series";
chart.GetNSeries().Get(0).SetName(val);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Series::SetName(const char16_t*) method


Gets or sets the name of the data series.

```cpp
void Aspose::Cells::Charts::Series::SetName(const char16_t *value)
```


## Examples


```cpp
//引用单元格的名称
chart.GetNSeries().Get(0).SetName(u"=A1");

//设置字符串为名称
chart.GetNSeries().Get(0).SetName(u"First Series");
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
