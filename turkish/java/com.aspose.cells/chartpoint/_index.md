---
title: "ChartPoint"
second_title: "Aspose.Cells for Java API Referansı"
description: "Grafikteki bir seride tek bir noktayı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

Grafikteki bir seride tek bir noktayı temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.PIE_EXPLODED, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Show Data Labels 
         chart.getNSeries().get(0).getDataLabels().setShowValue(true);
 
         for (int i = 0; i  <chart.getNSeries().get(0).getPoints().getCount(); i++)
         {
             //Get Data Point
             ChartPoint point = chart.getNSeries().get(0).getPoints().get(i);
             //Set Pir Explosion
             point.setExplosion(15);
             //Set Border Color
             point.getBorder().setColor(com.aspose.cells.Color.getRed());
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının x koordinatını alır. |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının y koordinatını alır. |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Chart.Calculate() metodunu çağırdıktan sonra pasta diliminin başlangıç noktasının x koordinatını alır. |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Chart.Calculate() metodunu çağırdıktan sonra pasta diliminin başlangıç noktasının y koordinatını alır. |
| [getArea()](#getArea--) | Alır [getArea()](../../com.aspose.cells/chartpoint\#getArea--). |
| [getBorder()](#getBorder--) | Alır [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Chart.Calculate() metodunu çağırdıktan sonra kenarlığın piksel cinsinden genişliğini alır. |
| [getBottomPointCount()](#getBottomPointCount--) | Chart.Calculate() metodunu çağırdıktan sonra alt noktaların sayısını alır. |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Chart.Calculate() metodunu çağırdıktan sonra şeklin alt noktasının x koordinatını alır. |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Chart.Calculate() metodunu çağırdıktan sonra şeklin alt noktasının y koordinatını alır. |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Bu grafik noktasına bağlı veri etiketini temsil eden bir [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) nesnesi döndürür. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Chart.Calculate() metodunu çağırdıktan sonra halka diliminin iç yarıçapını piksel cinsinden alır. |
| [getEndAngle()](#getEndAngle--) | Chart.Calculate() metodunu çağırdıktan sonra pasta diliminin bitiş açısını, x ekseninden saat yönünde derece cinsinden ölçer. |
| [getExplosion()](#getExplosion--) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının x koordinatını alır. |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının y koordinatını alır. |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Chart.Calculate() metodunu çağırdıktan sonra pasta diliminin başlangıç noktasının x koordinatını alır. |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Chart.Calculate() metodunu çağırdıktan sonra pasta diliminin başlangıç noktasının y koordinatını alır. |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Chart.Calculate() metodunu çağırdıktan sonra halka diliminin iç yarıçapını piksel cinsinden alır. |
| [getMarker()](#getMarker--) | Alır [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki nokta sayısını alır. |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki noktanın x koordinatını alır. |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki noktanın y koordinatını alır. |
| [getRadiusPx()](#getRadiusPx--) | Chart.Calculate() metodunu çağırdıktan sonra balon, pasta veya halka yarıçapını piksel cinsinden alır. |
| [getShadow()](#getShadow--) | Grafik noktasının gölgesi varsa doğru. |
| [getShapeHeight()](#getShapeHeight--) | Chart.Calculate() metodunu çağırdıktan sonra grafiğin yüksekliğinin 1/4000 birimindeki yüksekliği alır. |
| [getShapeHeightPx()](#getShapeHeightPx--) | Chart.Calculate() metodunu çağırdıktan sonra yüksekliği piksel cinsinden alır. |
| [getShapeProperties()](#getShapeProperties--) | ChartPoint'in görsel şekil özelliklerini tutan bir [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) nesnesini alır. |
| [getShapeWidth()](#getShapeWidth--) | Chart.Calculate() metodunu çağırdıktan sonra grafiğin genişliğinin 1/4000 birimindeki genişliği alır. |
| [getShapeWidthPx()](#getShapeWidthPx--) | Chart.Calculate() metodunu çağırdıktan sonra genişliği piksel cinsinden alır. |
| [getShapeX()](#getShapeX--) | Chart.Calculate() metodunu çağırdıktan sonra grafiğin genişliğinin 1/4000 birimindeki sol üst köşenin x koordinatını alır. |
| [getShapeXPx()](#getShapeXPx--) | Chart.Calculate() metodunu çağırdıktan sonra sol üst köşenin x koordinatını piksel cinsinden alır. |
| [getShapeY()](#getShapeY--) | Chart.Calculate() yöntemi çağrıldıktan sonra grafiğin yüksekliğinin 1/4000 biriminde üst sol köşenin y koordinatını alır. |
| [getShapeYPx()](#getShapeYPx--) | Chart.Calculate() yöntemi çağrıldıktan sonra üst sol köşenin y koordinatını piksel biriminde alır. |
| [getStartAngle()](#getStartAngle--) | Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin başlangıç açısını, x ekseninden saat yönünde derece cinsinden alır. |
| [getTopPointCount()](#getTopPointCount--) | Chart.Calculate() yöntemi çağrıldıktan sonra üst nokta sayısını alır. |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Chart.Calculate() yöntemi çağrıldıktan sonra şeklin üst noktasının x koordinatını alır. |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Chart.Calculate() yöntemi çağrıldıktan sonra şeklin üst noktasının y koordinatını alır. |
| [getXValue()](#getXValue--) | Grafik noktasının X değerini alır. |
| [getXValueType()](#getXValueType--) | Grafik noktasının X değer tipini alır. |
| [getYValue()](#getYValue--) | Grafik noktasının Y değerini alır. |
| [getYValueType()](#getYValueType--) | Grafik noktasının Y değer tipini alır. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Bu veri noktasının pasta içinde ikinci pasta ya da çubukta olup olmadığını gösteren bir değeri alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Bu veri noktasının pasta içinde ikinci pasta ya da çubukta olup olmadığını gösteren bir değeri ayarlar. |
| [setShadow(boolean value)](#setShadow-boolean-) | Grafik noktasının gölgesi varsa doğru. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Grafik noktasının X değerini ayarlar. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Grafik noktasının Y değerini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının x koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının y koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin başlangıç noktasının x koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin başlangıç noktasının y koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


Alır [getArea()](../../com.aspose.cells/chartpoint\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Alır [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


Chart.Calculate() metodunu çağırdıktan sonra kenarlığın piksel cinsinden genişliğini alır.

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


Chart.Calculate() metodunu çağırdıktan sonra alt noktaların sayısını alır.

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


Chart.Calculate() yöntemi çağrıldıktan sonra şeklin alt noktasının x koordinatını alır. 3D grafiklerine uygulanır: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


Chart.Calculate() yöntemi çağrıldıktan sonra şeklin alt noktasının y koordinatını alır. 3D grafiklerine uygulanır: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Bu grafik noktasına bağlı veri etiketini temsil eden bir [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--) nesnesi döndürür.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


Chart.Calculate() yöntemi çağrıldıktan sonra doughnut diliminin iç yarıçapını piksel biriminde alır. Doughnut grafiğine uygulanır.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş açısını, x ekseninden saat yönünde derece cinsinden alır. Pie grafiğine uygulanır.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının x koordinatını alır. Doughnut grafiklerine uygulanır.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının y koordinatını alır. Doughnut grafiğine uygulanır.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra pasta diliminin başlangıç noktasının x koordinatını alır. Doughnut grafiğine uygulanır.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


Chart.Calculate() metodunu çağırdıktan sonra pasta diliminin başlangıç noktasının y koordinatını alır. Doughnut grafiği için geçerlidir.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


Chart.Calculate() metodunu çağırdıktan sonra doughnut diliminin iç yarıçapını piksel biriminde alır. Doughnut grafiği için geçerlidir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen ChartPoint.DoughnutInnerRadius özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Alır [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki nokta sayısını alır. Yalnızca alan grafikleri için geçerlidir.

**Remarks**

Area 2D grafiği 1, Area 3D grafiği 2 döndürür.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki noktanın x koordinatını alır. Yalnızca Area grafiği için geçerlidir.

**Remarks**

Area 2D grafik: indeks 0. Area 3D grafik: indeks 0 veya 1.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki noktanın y koordinatını alır. Yalnızca Area grafiği için geçerlidir.

**Remarks**

Area 2D grafik: indeks 0. Area 3D grafik: indeks 0 veya 1.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


Chart.Calculate() metodunu çağırdıktan sonra balon, pasta veya halka yarıçapını piksel cinsinden alır.

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Grafik noktasının gölgesi varsa doğru.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


Chart.Calculate() metodunu çağırdıktan sonra grafiğin yüksekliğinin 1/4000 birimindeki yüksekliği alır.

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


Chart.Calculate() metodunu çağırdıktan sonra yüksekliği piksel cinsinden alır.

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


ChartPoint'in görsel şekil özelliklerini tutan bir [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) nesnesini alır.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


Chart.Calculate() metodunu çağırdıktan sonra grafiğin genişliğinin 1/4000 birimindeki genişliği alır.

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


Chart.Calculate() metodunu çağırdıktan sonra genişliği piksel cinsinden alır.

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


Chart.Calculate() metodunu çağırdıktan sonra grafiğin genişliğinin 1/4000 birimindeki sol üst köşenin x koordinatını alır.

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


Chart.Calculate() metodunu çağırdıktan sonra sol üst köşenin x koordinatını piksel cinsinden alır.

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


Chart.Calculate() yöntemi çağrıldıktan sonra grafiğin yüksekliğinin 1/4000 biriminde üst sol köşenin y koordinatını alır.

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


Chart.Calculate() yöntemi çağrıldıktan sonra üst sol köşenin y koordinatını piksel biriminde alır.

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


Chart.Calculate() metodunu çağırdıktan sonra pasta diliminin başlangıç açısını, x ekseninden saat yönünde derece cinsinden ölçerek alır. Pie grafiği için geçerlidir.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


Chart.Calculate() yöntemi çağrıldıktan sonra üst nokta sayısını alır.

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


Chart.Calculate() metodunu çağırdıktan sonra şeklin üst noktasının x koordinatını alır. 3D grafiklerde geçerlidir: Column3D, Bar3D, Cone, Cylinder, Pyramid ve Area3D.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


Chart.Calculate() metodunu çağırdıktan sonra şeklin üst noktasının y koordinatını alır. 3D grafiklerde geçerlidir: Column3D, Bar3D, Cone, Cylinder, Pyramid ve Area3D.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


Grafik noktasının X değerini alır.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


Grafik noktasının X değer tipini alır.

Bakınız [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


Grafik noktasının Y değerini alır.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


Grafik noktasının Y değer tipini alır.

Bakınız [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isInSecondaryPlot() {#isInSecondaryPlot--}
```
public boolean isInSecondaryPlot()
```


Bu veri noktasının pasta içinde ikinci pasta ya da çubukta olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzdesi olarak ifade edilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


Bu veri noktasının pasta içinde ikinci pasta ya da çubukta olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Grafik noktasının gölgesi varsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


Grafik noktasının X değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


Grafik noktasının Y değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

