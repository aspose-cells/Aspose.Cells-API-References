---
title: add_area yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
Doğrulamayı alana uygular.



```python
def add_area(self, cell_area):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| cell_area | [CellArea](/cells/tr/python-net/aspose.cells/cellarea) | Alan.|
###  Notlar

[Validation.add_area(cell_area)](/cells/tr/python-net/aspose.cells/validation/add_area) kullanmaya eşdeğerdir.
kesişme ve kenar kontrolü ile.

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
Doğrulamayı alana uygular.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| cell_area | [CellArea](/cells/tr/python-net/aspose.cells/cellarea) | Alan.|
| check_intersection | bool | Verilen alanın mevcut doğrulama alanları ile kesişiminin kontrol edilip edilmediği.<br/>Belirli bir alanda (veya bir bölümünde) bir doğrulama uygulanmışsa,<br/>daha sonra mevcut doğrulama ilk olarak verilen alandan kaldırılmalıdır.<br/>Aksi halde oluşturulan Validasyonlarda bozulmalar meydana gelebilir.<br/>Kullanıcı, eklenen alanın mevcut herhangi bir alanla kesişmediğinden eminse,<br/> bu parametre, performans değerlendirmesi için yanlış olarak ayarlanabilir.|
| check_edge | bool | Bu doğrulamanın uygulandığı alanların kenarlarını kontrol edin.<br/>Doğrulamanın dahili ayarları, uygulanan aralıkların sol üst köşesine bağlıdır.<br/>bu nedenle, verilen alan uygulanan aralıkların sol üst kısmı olacaksa,<br/>dahili ayarlar değiştirilip yeniden oluşturulmalıdır, aksi takdirde beklenmeyen sonuçlara neden olabilir.<br/>Kullanıcı, eklenen alanın sol üst alan olmadığından eminse,<br/> bu parametre, performans değerlendirmesi için yanlış olarak ayarlanabilir.|
###  Notlar

Bu yöntemde, verilen alandaki tüm eski doğrulamaları kaldıracağız.
Validation'ın uygulanan aralıklarından sol üstteki için, öncelikle StartRow'u en küçüktür,
ikinci olarak, StartColumn, aynı en küçük StartRow'a sahip alanların en küçüğüdür.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Validation](/cells/tr/python-net/aspose.cells/validation)
