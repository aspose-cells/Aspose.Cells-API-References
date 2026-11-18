---
title: "Chart Sınıfı"
linktitle: "Chart"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Chart sınıfı. Go dilinde chart'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/chart/
---

## Chart class

Tek bir Excel çizelgesini temsil eden nesneyi kapsüller.

```go

type Chart struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetStyle](./getstyle/) | Yerleşik stili alır ve ayarlar. |
| [SetStyle](./setstyle/) | Yerleşik stili alır ve ayarlar. |
| [GetChartObject](./getchartobject/) | chartShape'ı temsil eder; |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | Grafik PivotChart olduğunda yalnızca pivot grafik alan düğmelerinin gizlenip gizlenmeyeceğini gösterir. |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | Grafik PivotChart olduğunda yalnızca pivot grafik alan düğmelerinin gizlenip gizlenmeyeceğini gösterir. |
| [GetPivotOptions](./getpivotoptions/) | Grafikte görünen pivot kontrollerini belirtir |
| [GetPivotSource](./getpivotsource/) | Kaynak, pivot tablosunun verisidir. PivotSource boş değilse, grafik PivotChart'tır. |
| [SetPivotSource](./setpivotsource/) | Kaynak, pivot tablosunun verisidir. PivotSource boş değilse, grafik PivotChart'tır. |
| [IsCellReferedByChart](./iscellreferedbychart/) | Grafiğin referans verdiği hücrenin olup olmadığını döndürür. |
| [IsChartDataChanged](./ischartdatachanged/) | Bir grafiğin veri kaynağının değişip değişmediğini algılar. |
| [GetPlotBy](./getplotby/) | Satır mı sütun mu çizileceğini alır ve ayarlar. |
| [RefreshPivotData](./refreshpivotdata/) | Grafiğin verilerini pivot tablodan yeniler. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Boş hücrelerin nasıl çizileceğini alır ve ayarlar. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Boş hücrelerin nasıl çizileceğini alır ve ayarlar. |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir. |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | Yalnızca görünen hücrelerin çizilip çizilmeyeceğini gösterir. |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | #N/A değerinin boş bir değer olarak gösterilip gösterilmeyeceğini belirtir. |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | #N/A değerinin boş bir değer olarak gösterilip gösterilmeyeceğini belirtir. |
| [GetName](./getname/) | Grafiğin adını alır ve ayarlar. |
| [SetName](./setname/) | Grafiğin adını alır ve ayarlar. |
| [GetSizeWithWindow](./getsizewithwindow/) | Microsoft Excel, grafiği grafik sayfası penceresinin boyutuna göre yeniden boyutlandırıyorsa doğru. |
| [SetSizeWithWindow](./setsizewithwindow/) | Microsoft Excel, grafiği grafik sayfası penceresinin boyutuna göre yeniden boyutlandırıyorsa doğru. |
| [GetWorksheet](./getworksheet/) | Bu grafiği içeren çalışma sayfasını alır. |
| [GetShapes](./getshapes/) | Bu grafikteki tüm çizim şekillerini döndürür. |
| [GetPrintSize](./getprintsize/) | Yazdırılan grafik boyutunu alır ve ayarlar. |
| [SetPrintSize](./setprintsize/) | Yazdırılan grafik boyutunu alır ve ayarlar. |
| [ChangeTemplate](./changetemplate/) | Grafik türünü önceden ayarlanmış bir şablonla değiştir. |
| [GetType](./gettype/) | Bir grafiğin türünü alır veya ayarlar. |
| [SetType](./settype/) | Bir grafiğin türünü alır veya ayarlar. |
| [Move](./move/) | Grafiği belirtilen konuma taşır. |
| [GetNSeries](./getnseries/) | Grafikteki veri serilerini temsil eden bir SeriesCollection koleksiyonunu alır. |
| [GetFilteredNSeries](./getfilterednseries/) | Grafikte filtrelenen veri serilerini temsil eden bir SeriesCollection koleksiyonunu alır. |
| [GetTitle](./gettitle/) | Grafiğin başlığını alır. |
| [GetSubTitle](./getsubtitle/) | Grafiğin alt başlığını alır. Yalnızca ODS dosyalarına uygulanır. |
| [GetPlotArea](./getplotarea/) | Grafiğin eksen işaret etiketlerini içeren çizim alanını alır. |
| [GetChartArea](./getchartarea/) | Çalışma sayfasındaki grafik alanını alır. |
| [GetCategoryAxis](./getcategoryaxis/) | Grafiğin X eksenini alır. |
| [GetValueAxis](./getvalueaxis/) | Grafiğin Y eksenini alır. |
| [GetSecondValueAxis](./getsecondvalueaxis/) | Grafiğin ikinci Y eksenini alır. |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | Grafiğin ikinci X eksenini alır. |
| [GetSeriesAxis](./getseriesaxis/) | Grafiğin seri eksenini alır. |
| [GetLegend](./getlegend/) | Grafik açıklamasını alır. |
| [GetChartDataTable](./getchartdatatable/) | Grafik veri tablosunu temsil eder. |
| [GetShowLegend](./getshowlegend/) | Grafik açıklamasının gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [SetShowLegend](./setshowlegend/) | Grafik açıklamasının gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [IsRectangularCornered](./isrectangularcornered/) | Grafik alanının dikdörtgen köşeli olup olmadığını belirten bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [SetIsRectangularCornered](./setisrectangularcornered/) | Grafik alanının dikdörtgen köşeli olup olmadığını belirten bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [GetShowDataTable](./getshowdatatable/) | Grafiğin veri tablosu gösterip göstermediğini belirten bir değeri alır veya ayarlar. |
| [SetShowDataTable](./setshowdatatable/) | Grafiğin veri tablosu gösterip göstermediğini belirten bir değeri alır veya ayarlar. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) alır veya ayarlar. Yalnızca pasta, 3D pasta ve halka grafiklerine uygulanır, 0 ile 360 arasında. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden (dikeyden saat yönünde) alır veya ayarlar. Yalnızca pasta, 3D pasta ve halka grafiklerine uygulanır, 0 ile 360 arasında. |
| [GetGapWidth](./getgapwidth/) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [SetGapWidth](./setgapwidth/) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [GetGapDepth](./getgapdepth/) | 3D grafikte veri serileri arasındaki mesafeyi, işaretçi genişliğinin yüzdesi olarak alır veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [SetGapDepth](./setgapdepth/) | 3D grafikte veri serileri arasındaki mesafeyi, işaretçi genişliğinin yüzdesi olarak alır veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [Calculate](./calculate/) | Pozisyonları otomatik atanmışsa, çizim alanı ve eksenlerin özel konumlarını hesaplar. |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | Grafik alanının ve eksenlerin konumu otomatik atanmışsa, özel konumlarını Grafik Hesaplama Seçenekleri ile hesaplar. |
| [GetFloor](./getfloor/) | 3-B'li bir grafiğin duvarlarını temsil eden bir Floor nesnesi döndürür. |
| [GetWalls](./getwalls/) | 3-B'li bir grafiğin duvarlarını temsil eden bir Walls nesnesi döndürür. |
| [GetBackWall](./getbackwall/) | 3-B'li bir grafiğin arka duvarını temsil eden bir Walls nesnesi döndürür. |
| [GetSideWall](./getsidewall/) | 3-B'li bir grafiğin yan duvarını temsil eden bir Walls nesnesi döndürür. |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | 3-B'li bir grafikte ızgara çizgileri iki boyutlu çiziliyorsa doğru. |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | 3-B'li bir grafikte ızgara çizgileri iki boyutlu çiziliyorsa doğru. |
| [GetRotationAngle](./getrotationangle/) | 3-B'li grafik görünümünün dönüşünü temsil eder (grafik alanının z ekseni etrafındaki dönüşü, derece cinsinden). |
| [SetRotationAngle](./setrotationangle/) | 3-B'li grafik görünümünün dönüşünü temsil eder (grafik alanının z ekseni etrafındaki dönüşü, derece cinsinden). |
| [GetElevation](./getelevation/) | 3-B'li grafik görünümünün yüksekliğini derece cinsinden temsil eder. |
| [SetElevation](./setelevation/) | 3-B'li grafik görünümünün yüksekliğini derece cinsinden temsil eder. |
| [GetRightAngleAxes](./getrightangleaxes/) | Grafik eksenleri dik açıdaysa doğru. Yalnızca 3-B'li grafikler için geçerlidir (Column3D ve 3-B'li Pasta Grafikleri hariç). |
| [SetRightAngleAxes](./setrightangleaxes/) | Grafik eksenleri dik açıdaysa doğru. Yalnızca 3-B'li grafikler için geçerlidir (Column3D ve 3-B'li Pasta Grafikleri hariç). |
| [GetAutoScaling](./getautoscaling/) | Microsoft Excel bir 3-B'li grafiği, eşdeğer 2-B'li grafiğe daha yakın bir boyuta ölçeklendiriyorsa doğru. RightAngleAxes özelliği doğru olmalıdır. |
| [SetAutoScaling](./setautoscaling/) | Microsoft Excel bir 3-B'li grafiği, eşdeğer 2-B'li grafiğe daha yakın bir boyuta ölçeklendiriyorsa doğru. RightAngleAxes özelliği doğru olmalıdır. |
| [GetHeightPercent](./getheightpercent/) | 3-B'li bir grafiğin yüksekliğini, grafik genişliğinin yüzde olarak (%5 ile %500 arasında) döndürür veya ayarlar. |
| [SetHeightPercent](./setheightpercent/) | 3-B'li bir grafiğin yüksekliğini, grafik genişliğinin yüzde olarak (%5 ile %500 arasında) döndürür veya ayarlar. |
| [GetPerspective](./getperspective/) | 3-B'li grafik görünümü için perspektifi döndürür veya ayarlar. 0 ile 100 arasında olmalıdır. RightAngleAxes özelliği doğruysa bu özellik yok sayılır. |
| [SetPerspective](./setperspective/) | 3-B'li grafik görünümü için perspektifi döndürür veya ayarlar. 0 ile 100 arasında olmalıdır. RightAngleAxes özelliği doğruysa bu özellik yok sayılır. |
| [GetIs3D](./getis3d/) | Grafiğin 3-B'li bir grafik olup olmadığını gösterir. |
| [GetDepthPercent](./getdepthpercent/) | 3-B'li bir grafiğin derinliğini, grafik genişliğinin yüzde olarak (%20 ile %2000 arasında) temsil eder. |
| [SetDepthPercent](./setdepthpercent/) | 3-B'li bir grafiğin derinliğini, grafik genişliğinin yüzde olarak (%20 ile %2000 arasında) temsil eder. |
| [ToImage_String](./toimage_string/) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler. |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | Grafik görüntüsünü oluşturur ve belirtilen görüntü türünde bir dosyaya kaydeder. |
| [ToImage_Int64](./toimage_int64/) | Grafik görüntüsünü oluşturur ve JPEG formatında bir akışa kaydeder. |
| [ToImage_ImageType](./toimage_imagetype/) | Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder. |
| [ToPdf_String](./topdf_string/) | Grafiği bir PDF dosyasına kaydeder. |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Grafiği bir PDF dosyasına kaydeder. |
| [ToPdf](./topdf/) | Grafik PDF'sini oluşturur ve bir akışa kaydeder. |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Grafik PDF'sini oluşturur ve bir akışa kaydeder. |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler. |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder. |
| [GetActualSize](./getactualsize/) | Grafiğin gerçek boyutunu piksel biriminde alır. |
| [GetPlacement](./getplacement/) | Grafiğin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [SetPlacement](./setplacement/) | Grafiğin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [GetPageSetup](./getpagesetup/) | Bu grafikteki sayfa ayarı açıklamasını temsil eder. |
| [HasAxis](./hasaxis/) | Grafikte hangi eksenlerin bulunduğunu döndürür. |
| [SwitchRowColumn](./switchrowcolumn/) | Satır/sütun değiştirir. |
| [GetChartDataRange](./getchartdatarange/) | Grafiğin veri kaynağı aralığını alır. |
| [SetChartDataRange](./setchartdatarange/) | Bir grafik için veri aralığını belirtir. |
| [GetLine](./getline/) | Çizgiyi alır. |
