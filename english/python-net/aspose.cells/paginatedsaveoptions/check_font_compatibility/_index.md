---
title: check_font_compatibility property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 50
url: /python-net/aspose.cells/paginatedsaveoptions/check_font_compatibility/
is_root: false
---

## check_font_compatibility property


Indicates whether to check font compatibility for every character in text.

### Remarks 


The default value is true.
Disable this property may give better performance.
But when the default or specified font of text/character cannot be used to render it,
unreadable characters(such as block) maybe occur in the generated pdf.
For such situation user should keep this property as true so that
alternative font can be searched and used to render the text instead;

### See Also
* module [aspose.cells](../../)
* class [PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions)
