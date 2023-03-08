---
title: WorkbookMetadata الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
##  WorkbookMetadata الدرجة
يمثل البيانات الوصفية.



يكشف نوع WorkbookMetadata الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/ar/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) | إنشاء كائن البيانات الوصفية.|
| [WorkbookMetadata(stream, options)](/cells/ar/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) | إنشاء كائن البيانات الوصفية.|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [options](/cells/ar/python-net/aspose.cells.metadata/workbookmetadata/options) | يحصل على خيارات البيانات الوصفية.|
| [built_in_document_properties](/cells/ar/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |تقوم بارجاع مجموعة [DocumentProperty](/cells/ar/python-net/aspose.cells.properties/documentproperty) التي تمثل كل خصائص الوثيقة المضمنة لجدول حسابي.|
| [custom_document_properties](/cells/ar/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | تقوم بارجاع مجموعة [DocumentProperty](/cells/ar/python-net/aspose.cells.properties/documentproperty) التي تمثل كل خصائص الوثيقة المهيأة للجدول الحسابي.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [save(file_name)](/cells/ar/python-net/aspose.cells.metadata/workbookmetadata/save/#str) | احفظ البيانات الأولية المعدلة في الملف.|
| [save(stream)](/cells/ar/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) | احفظ البيانات الوصفية المعدلة في الدفق.|



###  مثال

يقوم المثال التالي بإنشاء WorkbookMetadata.

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells.metadata](..)
* فئة [DocumentProperty](/cells/ar/python-net/aspose.cells.properties/documentproperty)
