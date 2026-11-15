---
title: Aspose::Cells::Charts::ChartPointCollection class
linktitle: ChartPointCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartPointCollection class. Represents a collection that contains all the points in one series in C++.'
type: docs
weight: 1200
url: /tr/cpp/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class


Represents a collection that contains all the points in one series.

```cpp
class ChartPointCollection
```

## Methods

| Method | Description |
| --- | --- |
| [begin()](./begin/) | Returns an iterator to the beginning of the [ChartPointCollection](./). |
| [ChartPointCollection(ChartPointCollection_Impl* impl)](./chartpointcollection/) | Constructs from an implementation object. |
| [ChartPointCollection(const ChartPointCollection\& src)](./chartpointcollection/) | Copy constructor. |
| [Clear()](./clear/) | Remove all setting of the chart points. |
| [end()](./end/) | Returns an iterator to the end of the [ChartPointCollection](./). |
| [Get(int32_t index)](./get/) | Gets the [ChartPoint](../chartpoint/) element at the specified index in the series. |
| [GetCount()](./getcount/) | Gets the count of the chart point. |
| [GetEnumerator()](./getenumerator/) | Returns an enumerator for the entire [ChartPointCollection](./). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartPointCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Removes point at the index of the series. |
| [~ChartPointCollection()](./~chartpointcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;

//İlk çalışma sayfasının referansını elde etme
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//\"A1\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"A1").PutValue(50);

//\"A2\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"A2").PutValue(100);

//\"A3\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"A3").PutValue(150);

//\"B1\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"B1").PutValue(60);

//\"B2\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"B2").PutValue(32);

//\"B3\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"B3").PutValue(50);

//Çalışma sayfasına bir grafik ekleniyor
int chartIndex = worksheet.GetCharts().Add(ChartType::PieExploded, 5, 0, 25, 10);

//Yeni eklenen grafiğin örneğine erişiliyor
Chart chart = worksheet.GetCharts().Get(chartIndex);

//Grafiğe "A1" hücresinden "B3" hücresine kadar NSeries (grafik veri kaynağı) ekleme
chart.GetNSeries().Add(u"A1:B3", true);

//Veri Etiketlerini Göster
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

ChartPointCollection points = chart.GetNSeries().Get(0).GetPoints();

for (int i = 0; i < points.GetCount(); i++)
{
    //Veri Noktasını Al
    ChartPoint point = points.Get(i);
    //Pir Patlamasını Ayarla
    point.SetExplosion(15);
    //Kenarlık Rengini Ayarla
    point.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
}

//Excel dosyasını kaydetme
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
