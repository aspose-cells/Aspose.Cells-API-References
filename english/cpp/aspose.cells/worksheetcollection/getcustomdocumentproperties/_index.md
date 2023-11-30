---
title: Aspose::Cells::WorksheetCollection::GetCustomDocumentProperties method
linktitle: GetCustomDocumentProperties
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::WorksheetCollection::GetCustomDocumentProperties method. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet in C++.'
type: docs
weight: 3500
url: /cpp/aspose.cells/worksheetcollection/getcustomdocumentproperties/
---
## WorksheetCollection::GetCustomDocumentProperties method


Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.

```cpp
CustomDocumentPropertyCollection Aspose::Cells::WorksheetCollection::GetCustomDocumentProperties()
```


## Examples


```cpp
Aspose::Cells::Startup();
Workbook workbook;
workbook.GetWorksheets().GetCustomDocumentProperties().Add(u"Checked by", u"Jane");
Aspose::Cells::Cleanup();
```

## See Also

* Class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
