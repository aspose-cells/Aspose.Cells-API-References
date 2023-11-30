---
title: Aspose::Cells::Drawing::Shape::SetText method
linktitle: SetText
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetText method. Represents the string in this TextBox object in C++.'
type: docs
weight: 15600
url: /cpp/aspose.cells.drawing/shape/settext/
---
## Shape::SetText(const U16String\&) method


Represents the string in this [TextBox](../../textbox/) object.

```cpp
void Aspose::Cells::Drawing::Shape::SetText(const U16String &value)
```


## Examples


```cpp
U16String val = u"This is a test.";
if (shape.GetText().IsNull())
    shape.SetText(val);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetText(const char16_t*) method


Represents the string in this [TextBox](../../textbox/) object.

```cpp
void Aspose::Cells::Drawing::Shape::SetText(const char16_t *value)
```


## Examples


```cpp
if (shape.GetText().IsNull())
    shape.SetText(u"This is a test.");
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
