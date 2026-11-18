---
title: "ChartPoint Sınıfı"
linktitle: "ChartPoint"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ChartPoint sınıfı. Go'da chartpoint'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/chartpoint/
---

## ChartPoint class

Bir grafikte bir serideki tek bir noktayı temsil eder.

```go

type ChartPoint struct  {
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
| [GetExplosion](./getexplosion/) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzde olarak ifade edilir. |
| [SetExplosion](./setexplosion/) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzde olarak ifade edilir. |
| [GetShadow](./getshadow/) | Chartpoint'in bir gölgesi varsa doğru. |
| [SetShadow](./setshadow/) | Chartpoint'in bir gölgesi varsa doğru. |
| [GetBorder](./getborder/) | Satırı alır</see>. |
| [GetArea](./getarea/) | Alanı alır</see>. |
| [GetMarker](./getmarker/) | Marker'ı alır</see>. |
| [GetDataLabels](./getdatalabels/) | Bu grafik noktasına bağlı veri etiketini temsil eden bir DataLabels nesnesi döndürür. |
| [Get_YValue](./get_yvalue/) | Grafik noktasının Y değerini alır veya ayarlar. |
| [SetYValue](./setyvalue/) | Grafik noktasının Y değerini alır veya ayarlar. |
| [GetYValueType](./getyvaluetype/) | Grafik noktasının Y değer tipini alır. |
| [GetXValue](./getxvalue/) | Grafik noktasının X değerini alır veya ayarlar. |
| [SetXValue](./setxvalue/) | Grafik noktasının X değerini alır veya ayarlar. |
| [GetXValueType](./getxvaluetype/) | Grafik noktasının X değer tipini alır. |
| [GetShapeProperties](./getshapeproperties/) | ChartPoint'in görsel şekil özelliklerini tutan ShapePropertyCollection nesnesini alır. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | Bu veri noktasının pasta grafiğinin ikinci diliminde veya çubukta olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | Bu veri noktasının pasta grafiğinin ikinci diliminde veya çubukta olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [GetShapeX](./getshapex/) | Chart.Calculate() yöntemi çağrıldıktan sonra, grafiğin genişliğinin 1/4000 biriminde sol üst köşenin x koordinatını alır. |
| [GetShapeY](./getshapey/) | Chart.Calculate() yöntemi çağrıldıktan sonra, grafiğin yüksekliğinin 1/4000 biriminde sol üst köşenin y koordinatını alır. |
| [GetShapeWidth](./getshapewidth/) | Chart.Calculate() yöntemi çağrıldıktan sonra, grafiğin genişliğinin 1/4000 biriminde genişliği alır. |
| [GetShapeHeight](./getshapeheight/) | Chart.Calculate() yöntemi çağrıldıktan sonra, grafiğin yüksekliğinin 1/4000 biriminde yüksekliği alır. |
| [GetShapeXPx](./getshapexpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, piksel biriminde sol üst köşenin x koordinatını alır. |
| [GetShapeYPx](./getshapeypx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, piksel biriminde sol üst köşenin y koordinatını alır. |
| [GetShapeWidthPx](./getshapewidthpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, piksel biriminde genişliği alır. |
| [GetShapeHeightPx](./getshapeheightpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, piksel biriminde yüksekliği alır. |
| [GetBorderWidthPx](./getborderwidthpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, piksel biriminde kenarlık genişliğini alır. |
| [GetRadiusPx](./getradiuspx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, piksel biriminde balon, pasta veya halka yarıçapını alır. |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Chart.Calculate() yöntemi çağrıldıktan sonra, piksel biriminde halka diliminin iç yarıçapını alır. Doughnut grafiği için geçerlidir. |
| [GetStartAngle](./getstartangle/) | Chart.Calculate() yöntemi çağrıldıktan sonra, x ekseninden saat yönünde derece cinsinden ölçülen pasta diliminin başlangıç açısını alır. Pie grafiği için geçerlidir. |
| [GetEndAngle](./getendangle/) | Chart.Calculate() yöntemi çağrıldıktan sonra, x ekseninden saat yönünde derece cinsinden ölçülen pasta diliminin bitiş açısını alır. Pie grafiği için geçerlidir. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, pasta diliminin başlangıç noktasının x koordinatını alır. Pie ve Doughnut grafiklerinde geçerlidir. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, pasta diliminin başlangıç noktasının y koordinatını alır. Pie ve Doughnut grafiği için geçerlidir. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, pasta diliminin bitiş noktasının x koordinatını alır. Pie ve Doughnut grafiklerinde geçerlidir. |
| [GetArcEndPointYPx](./getarcendpointypx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, pasta diliminin bitiş noktasının y koordinatını alır. Pie ve Doughnut grafiği için geçerlidir. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, pasta diliminin başlangıç noktasının x koordinatını alır. Doughnut grafiği için geçerlidir. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Chart.Calculate() yöntemi çağrıldıktan sonra, pasta diliminin başlangıç noktasının y koordinatını alır. Doughnut grafiği için geçerlidir. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Pasta diliminin bitiş noktasının x koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. Donut grafiklerine uygulanır. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Pasta diliminin bitiş noktasının y koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. Donut grafiğine uygulanır. |
| [GetTopPointCount](./gettoppointcount/) | Chart.Calculate() metodunu çağırdıktan sonra üst nokta sayısını alır. |
| [GetTopPointXPx](./gettoppointxpx/) | Şeklin üst noktasının x koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. 3D grafiklerine uygulanır: Column3D, Bar3D, Cone, Cylinder, Pyramid ve Area3D |
| [GetTopPointYPx](./gettoppointypx/) | Şeklin üst noktasının y koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. 3D grafiklerine uygulanır: Column3D, Bar3D, Cone, Cylinder, Pyramid ve Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | Chart.Calculate() metodunu çağırdıktan sonra alt nokta sayısını alır. |
| [GetBottomPointXPx](./getbottompointxpx/) | Şeklin alt noktasının x koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. 3D grafiklerine uygulanır: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetBottomPointYPx](./getbottompointypx/) | Şeklin alt noktasının y koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. 3D grafiklerine uygulanır: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki nokta sayısını alır. Yalnızca alan grafiklerine uygulanır. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Kategori eksenindeki noktanın x koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. Yalnızca Alan grafiğine uygulanır. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Kategori eksenindeki noktanın y koordinatını Chart.Calculate() metodunu çağırdıktan sonra alır. Yalnızca Alan grafiğine uygulanır. |
