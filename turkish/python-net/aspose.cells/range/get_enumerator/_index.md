---
title: get_enumerator yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 90
url: /tr/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Bu Aralıktaki hücreler için Numaralandırıcıyı alır.


###  İadeler

Hücre numaralandırıcı


```python
def get_enumerator(self):
    ...
```


###  Notlar

Döndürülen Numaralandırıcı tarafından öğeler arasında geçiş yapılırken, hücre koleksiyonu
değiştirilmemelidir (yeni Cell/Row'un başlatılmasına veya mevcut Cell/Row'un silinmesine neden olacak işlemler gibi).
Aksi takdirde numaralandırıcı tüm hücreleri doğru şekilde geçemeyebilir (bazı öğeler tekrar tekrar geçilebilir veya atlanabilir).
###  örnekler

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)
