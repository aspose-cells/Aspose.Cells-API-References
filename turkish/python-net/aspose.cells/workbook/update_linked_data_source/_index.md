---
title: update_linked_data_source yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 410
url: /tr/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
Bu çalışma kitabı başka veri kaynaklarına harici bağlantılar içeriyorsa,
Aspose.Cells en son verileri almaya çalışacak.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| external_workbooks | list | Dış çalışma kitaplarına bu çalışma kitabı tarafından başvurulur.<br/>Eğer null ise, doğrudan harici bağlantılı dosyaları açacağız.<br/>Eğer boş değilse,<br/>önce dizideki harici bağlantının olup olmadığını kontrol edeceğiz;<br/> değilse, harici bağlantılı dosyaları tekrar açacağız.|
###  Notlar

Formülleri hesaplamadan önce yöntem çağrılmazsa,
Aspose.Cells önceki bilgileri kullanacaktır (dosyada önbelleğe alınmış);
 Lütfen CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath'i ayarlayın.
Ve bu çalışma kitabı bir akıştan ise, lütfen Workbook.FilePath'i ayarlayın.
aksi halde Aspose.Cells bazen dış bağlantının tam yolunu alamıyordu.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
