---
title: ExternalLink sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 560
url: /tr/python-net/aspose.cells/externallink/
is_root: false
---
##  ExternalLink sınıfı
Çalışma kitabındaki harici bir bağlantıyı temsil eder.



ExternalLink türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [type](/cells/tr/python-net/aspose.cells/externallink/type) | Dış bağlantının türünü alır.|
| [original_data_source](/cells/tr/python-net/aspose.cells/externallink/original_data_source) | Dış bağlantının saklanan veri kaynağını temsil eder.|
| [data_source](/cells/tr/python-net/aspose.cells/externallink/data_source) | Dış bağlantının veri kaynağını temsil eder.|
| [is_referred](/cells/tr/python-net/aspose.cells/externallink/is_referred) | Bu harici bağlantıya başkaları tarafından başvuruda bulunulup bulunulmadığını gösterir.|
| [is_visible](/cells/tr/python-net/aspose.cells/externallink/is_visible) | Bu harici bağlantının MS Excel'de görünüp görünmediğini gösterir.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add_external_name(text, refer_to)](/cells/tr/python-net/aspose.cells/externallink/add_external_name/#str-str) | Harici bir ad ekler.|



###  Örnek

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Get External Link
externalLink = workbook.worksheets.external_links[0]
# Change External Link's Data Source
externalLink.data_source = "d:\\link.xls"

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
