---
title: ExternalLinkCollection sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 570
url: /tr/python-net/aspose.cells/externallinkcollection/
is_root: false
---
##  ExternalLinkCollection sınıf
Bir çalışma kitabındaki dış bağlantılar koleksiyonunu temsil eder.



ExternalLinkCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [count](/cells/tr/python-net/aspose.cells/externallinkcollection/count) | Koleksiyonda fiilen bulunan öğelerin sayısını alır.|



Belirtilen dizindeki [ExternalLink](/cells/tr/python-net/aspose.cells/externallink) öğesini alır.
###  İndeksleyici
| İsim| Tanım|
| :- | :- |
| [index] | Öğenin sıfır tabanlı dizini.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(file_name, sheet_names)](/cells/tr/python-net/aspose.cells/externallinkcollection/add/#str-list) | Harici bir bağlantı ekler.|
| [add(directory_type, file_name, sheet_names)](/cells/tr/python-net/aspose.cells/externallinkcollection/add/#DirectoryType-str-list) | Harici bir bağlantı ekleyin.|
| [clear()](/cells/tr/python-net/aspose.cells/externallinkcollection/clear/#) | Tüm harici bağlantıları kaldırır.|
| [clear(update_references_as_local)](/cells/tr/python-net/aspose.cells/externallinkcollection/clear/#bool) | Tüm harici bağlantıları kaldırır.|
| [remove_at(index)](/cells/tr/python-net/aspose.cells/externallinkcollection/remove_at/#int) | Belirtilen dış bağlantıyı çalışma kitabından kaldırır.|
| [remove_at(index, update_references_as_local)](/cells/tr/python-net/aspose.cells/externallinkcollection/remove_at/#int-bool) | Belirtilen dış bağlantıyı çalışma kitabından kaldırır.|



###  Örnek

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Change external link data source
workbook.worksheets.external_links[0].data_source = "d:\\link.xls"

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [ExternalLink](/cells/tr/python-net/aspose.cells/externallink)
