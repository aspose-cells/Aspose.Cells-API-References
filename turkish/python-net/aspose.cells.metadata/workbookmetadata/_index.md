---
title: WorkbookMetadata sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
##  WorkbookMetadata sınıf
Meta verileri temsil eder.



WorkbookMetadata türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/tr/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) | Meta veri nesnesini oluşturun.|
| [WorkbookMetadata(stream, options)](/cells/tr/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) | Meta veri nesnesini oluşturun.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [options](/cells/tr/python-net/aspose.cells.metadata/workbookmetadata/options) | Meta veri seçeneklerini alır.|
| [built_in_document_properties](/cells/tr/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |Elektronik tablonun tüm yerleşik belge özelliklerini temsil eden bir [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty) koleksiyonunu döndürür.|
| [custom_document_properties](/cells/tr/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | Elektronik tablonun tüm özel belge özelliklerini temsil eden bir [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty) koleksiyonunu döndürür.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [save(file_name)](/cells/tr/python-net/aspose.cells.metadata/workbookmetadata/save/#str) | Değiştirilen meta verileri dosyaya kaydedin.|
| [save(stream)](/cells/tr/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) | Değiştirilen meta verileri akışa kaydedin.|



###  Örnek

Aşağıdaki örnek bir WorkbookMetadata oluşturur.

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.metadata](..)
* sınıf [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty)
