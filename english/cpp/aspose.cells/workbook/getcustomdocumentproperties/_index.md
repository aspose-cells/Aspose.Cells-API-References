---
title: Aspose::Cells::Workbook::GetCustomDocumentProperties method
linktitle: GetCustomDocumentProperties
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Workbook::GetCustomDocumentProperties method. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet in C++.'
type: docs
weight: 5800
url: /cpp/aspose.cells/workbook/getcustomdocumentproperties/
---
## Workbook::GetCustomDocumentProperties method


Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.

```cpp
CustomDocumentPropertyCollection Aspose::Cells::Workbook::GetCustomDocumentProperties()
```


## Examples


```cpp
Aspose::Cells::Startup();
Workbook excel;
excel.GetCustomDocumentProperties().Add(u"Checked by", u"Jane");
Aspose::Cells::Cleanup();
```

## See Also

* Class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
