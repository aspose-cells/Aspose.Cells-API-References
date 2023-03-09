---
title: process_cell yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
Bir hücreyi işlemeye başlar.


###  İadeler

bu hücrenin geçerli sayfanın hücre modelinde tutulması gerekip gerekmediği.
Genellikle, tüm hücrelerin işlendikten sonra bellekte tutulmaması ve ardından bellek kaydedilmesi için yanlış olmalıdır.
Kullanıcının tüm çalışma kitabı işlendikten sonra bazı hücrelere erişmesi gibi bazı özel amaçlar için,
kullanıcı, bu özel hücreleri Cells modelinde tutmak için bu yöntemin true dönüşünü sağlayabilir ve bunlara daha sonra Cells[satır, sütun] gibi API'ler aracılığıyla erişebilir.
Ancak, hücre verilerini Cells modelinde tutmak daha fazla bellek gerektirir ve tüm hücreler tutulursa şablon dosyasını okur
LightCells modunda, normal şekilde okumakla aynı hale gelecektir.


```python
def process_cell(self, cell):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| cell | [Cell](/cells/tr/python-net/aspose.cells/cell) | Cell şu anda işlenmekte olan nesne|
###  Notlar

Bir hücrenin verileri okunduktan sonra çağrılacaktır.


###  Ayrıca bakınız

* modül [aspose.cells](../../)
* sınıf [LightCellsDataHandler](/cells/tr/python-net/aspose.cells/lightcellsdatahandler)
