---
title: "Workbook.getBuiltInDocumentProperties"
linktitle: "getBuiltInDocumentProperties"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet."
type: docs
weight: 260
url: /nodejs/aspose.cells/workbook/getbuiltindocumentproperties/
---

## getBuiltInDocumentProperties()

Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: TitleSubjectAuthorKeywordsCommentsTemplateLast AuthorRevision NumberApplication NameLast Print DateCreation DateLast Save TimeTotal Editing TimeNumber of PagesNumber of WordsNumber of CharactersSecurityCategoryFormatManagerCompanyNumber of BytesNumber of LinesNumber of ParagraphsNumber of SlidesNumber of NotesNumber of Hidden SlidesNumber of Multimedia Clips

**Example:**

```js
var doc = workbook.getBuiltInDocumentProperties().get("Author");
doc.setValue("John Smith");
```
