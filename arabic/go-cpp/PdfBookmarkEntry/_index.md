---
title: "PdfBookmarkEntry فئة"
linktitle: "PdfBookmarkEntry"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "PdfBookmarkEntry فئة. يغلف الكائن الذي يمثل pdfbookmarkentry في Go."
type: docs
weight: 200
url: /ar/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry هو إدخال في إشارة مرجعية PDF. إذا كانت خاصية Text في المثيل الحالي فارغة أو \"\", سيتم إخفاء المثيل الحالي وسيتم إدراج العناصر الفرعية في المستوى الحالي.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetText](./gettext/) | عنوان العلامة المرجعية. |
| [SetText](./settext/) | عنوان العلامة المرجعية. |
| [GetDestination](./getdestination/) | الخلية التي يرتبط بها رابط العلامة المرجعية. |
| [SetDestination](./setdestination/) | الخلية التي يرتبط بها رابط العلامة المرجعية. |
| [GetDestinationName](./getdestinationname/) | يحصل أو يعيّن اسم الوجهة. |
| [SetDestinationName](./setdestinationname/) | يحصل أو يعيّن اسم الوجهة. |
| [IsOpen](./isopen/) | عند كون هذه الخاصية صحيحة، سيتوسع إدخال العلامة المرجعية، وإلا سيتقلص. |
| [SetIsOpen](./setisopen/) | عند كون هذه الخاصية صحيحة، سيتوسع إدخال العلامة المرجعية، وإلا سيتقلص. |
| [IsCollapse](./iscollapse/) | عند كون هذه الخاصية صحيحة، سيتقلص إدخال العلامة المرجعية، وإلا سيتوسع. |
| [SetIsCollapse](./setiscollapse/) | عند كون هذه الخاصية صحيحة، سيتقلص إدخال العلامة المرجعية، وإلا سيتوسع. |
