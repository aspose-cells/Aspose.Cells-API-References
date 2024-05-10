---
title: Aspose::Cells::HtmlSaveOptions::SetCssStyles method
linktitle: SetCssStyles
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::HtmlSaveOptions::SetCssStyles method. Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True in C++.'
type: docs
weight: 12000
url: /cpp/aspose.cells/htmlsaveoptions/setcssstyles/
---
## HtmlSaveOptions::SetCssStyles(const U16String\&) method


Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True.

```cpp
void Aspose::Cells::HtmlSaveOptions::SetCssStyles(const U16String &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
HtmlSaveOptions opt;
U16String css = u"body { padding: 5px }";
opt.SetCssStyles(css);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [HtmlSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## HtmlSaveOptions::SetCssStyles(const char16_t*) method


Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True.

```cpp
void Aspose::Cells::HtmlSaveOptions::SetCssStyles(const char16_t *value)
```


## Examples


```cpp
Aspose::Cells::Startup();
HtmlSaveOptions opt;
opt.SetCssStyles(u"body { padding: 5px }");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [HtmlSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
