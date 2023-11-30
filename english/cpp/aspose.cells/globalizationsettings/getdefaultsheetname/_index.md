---
title: Aspose::Cells::GlobalizationSettings::GetDefaultSheetName method
linktitle: GetDefaultSheetName
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::GlobalizationSettings::GetDefaultSheetName method. Gets the default sheet name for adding worksheet automatically. Default is "Sheet" in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings::GetDefaultSheetName method


Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

```cpp
virtual U16String Aspose::Cells::GlobalizationSettings::GetDefaultSheetName()
```


## ReturnValue

the default sheet name for adding worksheet automatically
## Remarks



The automatically added(such as by [WorksheetCollection.Add()](../../worksheetcollection/add/)) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".
## See Also

* Class [U16String](../../u16string/)
* Class [GlobalizationSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
