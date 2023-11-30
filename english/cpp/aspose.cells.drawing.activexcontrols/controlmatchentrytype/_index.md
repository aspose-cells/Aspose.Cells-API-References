---
title: Aspose::Cells::Drawing::ActiveXControls::ControlMatchEntryType enum
linktitle: ControlMatchEntryType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ActiveXControls::ControlMatchEntryType enum. Represents how a ListBox or ComboBox searches its list as the user types in C++.'
type: docs
weight: 1900
url: /cpp/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enum


Represents how a [ListBox](../../aspose.cells.drawing/listbox/) or [ComboBox](../../aspose.cells.drawing/combobox/) searches its list as the user types.

```cpp
enum class ControlMatchEntryType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| FirstLetter | 0 | The control searches for the next entry that starts with the character entered. Repeatedly typing the same letter cycles through all entries beginning with that letter. |
| Complete | 1 | As each character is typed, the control searches for an entry matching all characters entered. |
| None | 2 | The list will not be searched when characters are typed. |

## See Also

* Namespace [Aspose::Cells::Drawing::ActiveXControls](../)
* Library [Aspose.Cells for C++](../../)
