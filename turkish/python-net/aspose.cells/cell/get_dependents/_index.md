---
title: get_dependents yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 90
url: /tr/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
Formülü doğrudan bu hücreye başvuran tüm hücreleri alın.



```python
def get_dependents(self, is_all):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| is_all | bool | Diğer çalışma sayfalarındaki formülleri kontrol edip etmeyeceğini gösterir.|
###  Notlar

* Bu hücreyi içeren bir başvuru bir hücrenin formülünde görünürse, o hücre şu şekilde alınır:

Bu hücrenin bağımlısı, referans veya bu hücrenin hesaplama yapılırken kullanılıp kullanılmadığına bakılmaksızın.
Örneğin "=EĞER(DOĞRU,A1,A2)" formülündeki A2 hücresi hesaplama yapılırken kullanılmasa da,
Bu formül yine A2'nin bağımlısı olarak alınır.
Hesaplanan sonuçları bu hücreye bağlı olan formülleri almak için lütfen [Cell.get_dependents_in_calculation(recursive)](/cells/tr/python-net/aspose.cells/cell/get_dependents_in_calculation)'i kullanın. Bir hücre için bağımlıları izlerken, çalışma kitabındaki veya çalışma sayfasındaki tüm formüller analiz edilecek ve kontrol edilecektir.
Bu nedenle, zaman alan bir süreçtir.Kullanıcının çok sayıda hücre için bağımlıları izlemesi gerekiyorsa, bu yöntemi kullanmak
düşük performansa neden olur. Performansı değerlendirmek için kullanıcı bunun yerine [Cell.get_dependents_in_calculation(recursive)](/cells/tr/python-net/aspose.cells/cell/get_dependents_in_calculation)'i kullanmalıdır.
Veya kullanıcı önce [Cell.get_precedents()](/cells/tr/python-net/aspose.cells/cell/get_precedents) ile tüm hücrelerin emsal haritasını toplayabilir,
ve ardından emsal haritasına göre bağımlılar haritasını oluşturun.

* Bu hücreyi içeren bir başvuru bir hücrenin formülünde görünürse, o hücre şu şekilde alınır:
Bu hücrenin bağımlısı, referans veya bu hücrenin hesaplama yapılırken kullanılıp kullanılmadığına bakılmaksızın.
Örneğin "=EĞER(DOĞRU,A1,A2)" formülündeki A2 hücresi hesaplama yapılırken kullanılmasa da,
Bu formül yine A2'nin bağımlısı olarak alınır.
Hesaplanan sonuçları bu hücreye bağlı olan formülleri almak için lütfen [Cell.get_dependents_in_calculation(recursive)](/cells/tr/python-net/aspose.cells/cell/get_dependents_in_calculation)'i kullanın. Bir hücre için bağımlıları izlerken, çalışma kitabındaki veya çalışma sayfasındaki tüm formüller analiz edilecek ve kontrol edilecektir.
Bu nedenle, zaman alan bir süreçtir.Kullanıcının çok sayıda hücre için bağımlıları izlemesi gerekiyorsa, bu yöntemi kullanmak
düşük performansa neden olur. Performansı değerlendirmek için kullanıcı bunun yerine [Cell.get_dependents_in_calculation(recursive)](/cells/tr/python-net/aspose.cells/cell/get_dependents_in_calculation)'i kullanmalıdır.
Veya kullanıcı önce [Cell.get_precedents()](/cells/tr/python-net/aspose.cells/cell/get_precedents) ile tüm hücrelerin emsal haritasını toplayabilir,
ve ardından emsal haritasına göre bağımlılar haritasını oluşturun.

* Bu hücreyi içeren bir başvuru bir hücrenin formülünde görünürse, o hücre şu şekilde alınır:
Bu hücrenin bağımlısı, referans veya bu hücrenin hesaplama yapılırken kullanılıp kullanılmadığına bakılmaksızın.
Örneğin "=EĞER(DOĞRU,A1,A2)" formülündeki A2 hücresi hesaplama yapılırken kullanılmasa da,
Bu formül yine A2'nin bağımlısı olarak alınır.
Hesaplanan sonuçları bu hücreye bağlı olan formülleri almak için lütfen [Cell.get_dependents_in_calculation(recursive)](/cells/tr/python-net/aspose.cells/cell/get_dependents_in_calculation)'i kullanın. Bir hücre için bağımlıları izlerken, çalışma kitabındaki veya çalışma sayfasındaki tüm formüller analiz edilecek ve kontrol edilecektir.
Bu nedenle, zaman alan bir süreçtir.Kullanıcının çok sayıda hücre için bağımlıları izlemesi gerekiyorsa, bu yöntemi kullanmak
düşük performansa neden olur. Performansı değerlendirmek için kullanıcı bunun yerine [Cell.get_dependents_in_calculation(recursive)](/cells/tr/python-net/aspose.cells/cell/get_dependents_in_calculation)'i kullanmalıdır.
Veya kullanıcı önce [Cell.get_precedents()](/cells/tr/python-net/aspose.cells/cell/get_precedents) ile tüm hücrelerin emsal haritasını toplayabilir,
ve ardından emsal haritasına göre bağımlılar haritasını oluşturun.
###  örnekler

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
    print(dependents[i].name)

```



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
