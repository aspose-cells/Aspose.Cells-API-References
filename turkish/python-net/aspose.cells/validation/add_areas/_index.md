---
title: add_areas yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells/validation/add_areas/
is_root: false
---
##  add_areas(areas, check_intersection, check_edge) {#list-bool-bool}
Doğrulamayı verilen alanlara uygular.



```python
def add_areas(self, areas, check_intersection, check_edge):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| areas | list | Alanlar.|
| check_intersection | bool | Verilen alanın mevcut doğrulama alanları ile kesişiminin kontrol edilip edilmediği.<br/>Belirli bir alanda (veya bir bölümünde) bir doğrulama uygulanmışsa,<br/>daha sonra mevcut doğrulama ilk olarak verilen alandan kaldırılmalıdır.<br/>Aksi takdirde, oluşturulan Doğrulamalar bozulmaya neden olabilir.<br/>Kullanıcı, eklenen tüm alanların mevcut herhangi bir alanla kesişmediğinden eminse,<br/> Bu parametre, performans değerlendirmesi için yanlış olarak ayarlanabilir.|
| check_edge | bool | Bu doğrulamanın uygulandığı alanların kenarlarını kontrol edin.<br/>Doğrulamanın dahili ayarları, uygulanan aralıkların sol üst köşesine bağlıdır.<br/>bu nedenle, verilen alanlardan biri uygulanan aralıkların sol üst kısmı olacaksa,<br/>dahili ayarlar değiştirilip yeniden oluşturulmalıdır, aksi takdirde beklenmeyen sonuçlara neden olabilir.<br/>Kullanıcı, eklenen alanlardan hiçbirinin sol üstte olmadığından eminse,<br/> Bu parametre, performans değerlendirmesi için yanlış olarak ayarlanabilir.|
###  Notlar

Bu yöntemde, belirli bir alandaki tüm eski doğrulamaları kaldıracağız.
Validation'ın uygulanan aralıklarından sol üstteki için, öncelikle StartRow'u en küçüktür,
ikinci olarak, StartColumn, aynı en küçük StartRow'a sahip alanların en küçüğüdür.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Validation](/cells/tr/python-net/aspose.cells/validation)
