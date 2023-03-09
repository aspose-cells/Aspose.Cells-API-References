---
title: get_precedents yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 180
url: /tr/python-net/aspose.cells/cell/get_precedents/
is_root: false
---
##  get_precedents() {#}
Bu hücrenin formülünde görünen tüm başvuruları alır.


###  İadeler

Bu hücrenin formülünde görünen tüm referansların toplanması.


```python
def get_precedents(self):
    ...
```


###  Notlar

* Bu bir formül hücresi değilse null döndürür. Bu hücrenin formülünde görünen tüm başvurular, hesaplama sırasında başvurulsa da başvurulmasa da döndürülür.

Örneğin "=EĞER(DOĞRU,A1,A2)" formülündeki A2 hücresi hesaplama yapılırken kullanılmasa da,
hala formülün emsalleri olarak alınmaktadır. Yalnızca hesaplamayı etkileyen referansları almak için lütfen [Cell.get_precedents_in_calculation()](/cells/tr/python-net/aspose.cells/cell/get_precedents_in_calculation)'i kullanın.

* Bu bir formül hücresi değilse null döndürür. Bu hücrenin formülünde görünen tüm başvurular, hesaplama sırasında başvurulsa da başvurulmasa da döndürülür.
Örneğin "=EĞER(DOĞRU,A1,A2)" formülündeki A2 hücresi hesaplama yapılırken kullanılmasa da,
hala formülün emsalleri olarak alınmaktadır. Yalnızca hesaplamayı etkileyen referansları almak için lütfen [Cell.get_precedents_in_calculation()](/cells/tr/python-net/aspose.cells/cell/get_precedents_in_calculation)'i kullanın.

* Bu bir formül hücresi değilse null döndürür. Bu hücrenin formülünde görünen tüm başvurular, hesaplama sırasında başvurulsa da başvurulmasa da döndürülür.
Örneğin "=EĞER(DOĞRU,A1,A2)" formülündeki A2 hücresi hesaplama yapılırken kullanılmasa da,
hala formülün emsalleri olarak alınmaktadır. Yalnızca hesaplamayı etkileyen referansları almak için lütfen [Cell.get_precedents_in_calculation()](/cells/tr/python-net/aspose.cells/cell/get_precedents_in_calculation)'i kullanın.
###  Örnek

```python
from aspose.cells import CellsHelper, Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1"
areas = cells.get("A1").get_precedents()
for i in range(len(areas)):
    area = areas[i]
    stringBuilder = []
    if area.is_external_link:
        stringBuilder.append("[")
        stringBuilder.append(area.external_file_name)
        stringBuilder.append("]")
    stringBuilder.append(area.sheet_name)
    stringBuilder.append("!")
    stringBuilder.append(CellsHelper.cell_index_to_name(area.start_row, area.start_column))
    if area.is_area:
        stringBuilder.append(":")
        stringBuilder.append(CellsHelper.cell_index_to_name(area.end_row, area.end_column))
    print("".join(stringBuilder))

```



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
