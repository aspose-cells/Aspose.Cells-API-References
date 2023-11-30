---
title: Aspose::Cells::PaginatedSaveOptions::SetCheckFontCompatibility method
linktitle: SetCheckFontCompatibility
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetCheckFontCompatibility method. Indicates whether to check font compatibility for every character in text in C++.'
type: docs
weight: 1000
url: /cpp/aspose.cells/paginatedsaveoptions/setcheckfontcompatibility/
---
## PaginatedSaveOptions::SetCheckFontCompatibility method


Indicates whether to check font compatibility for every character in text.

```cpp
void Aspose::Cells::PaginatedSaveOptions::SetCheckFontCompatibility(bool value)
```

## Remarks


The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead; 
## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
