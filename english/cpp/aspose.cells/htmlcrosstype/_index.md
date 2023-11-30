---
title: Aspose::Cells::HtmlCrossType enum
linktitle: HtmlCrossType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::HtmlCrossType enum. Represents five types of html cross string in C++.'
type: docs
weight: 21200
url: /cpp/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enum


Represents five types of html cross string.

```cpp
enum class HtmlCrossType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Default | 0 | Display like MS Excel,depends on the next cell. If the next cell is null,the string will cross,or it will be truncated. |
| MSExport | 1 | Display the string like MS Excel exporting html. |
| Cross | 2 | Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
| CrossHideRight | 3 | Display HTML cross string and hide the right string when the texts overlap. |
| FitToCell | 4 | Only displaying the string within the width of cell. |

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
