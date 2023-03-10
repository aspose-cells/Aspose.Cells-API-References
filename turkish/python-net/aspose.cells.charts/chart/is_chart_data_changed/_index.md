---
title: is_chart_data_changed yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 70
url: /tr/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
Bir grafiğin veri kaynağının değişip değişmediğini algılar.


###  İadeler

Grafik değiştiyse true döndürür, aksi halde false döndürür


```python
def is_chart_data_changed(self):
    ...
```


###  Notlar

Yöntem, grafiği görüntü formatına dönüştürmeden önce grafiğin veri kaynağındaki değişiklikleri algılar.
İlk Chart.toImage çağrısında, grafik kaynak verileri (örn. XValuesParseData, ValuesParseData) kaydedilecektir.
Chart.toImage yöntemini yeniden çağırmadan önce, Chart'ın yeniden oluşturulması gerekip gerekmediğini kontrol etmek için IsChartDataChanged yöntemini çağırın.


###  Ayrıca bakınız
* modül [aspose.cells.charts](../../)
* sınıf [Chart](/cells/tr/python-net/aspose.cells.charts/chart)
