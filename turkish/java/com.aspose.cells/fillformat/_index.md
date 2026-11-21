---
title: "FillFormat"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir şekil için doldurma biçimlendirmesini temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/fillformat/
---

**Inheritance:**
java.lang.Object
```
public class FillFormat
```

Bir şekil için doldurma biçimlendirmesini temsil eden nesneyi kapsüller.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Filling the area of the 2nd NSeries with a gradient
         chart.getNSeries().get(seriesIndex).getArea().getFillFormat().setOneColorGradient(Color.getLime(), 1, GradientStyleType.HORIZONTAL, 1);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | Dolgu tipini alır |
| [getGradientColor1()](#getGradientColor1--) | Belirtilen dolgu için geçiş rengi 1'i döndürür. |
| [getGradientColor2()](#getGradientColor2--) | Belirtilen dolgu için geçiş rengi 2'yi döndürür. |
| [getGradientColorType()](#getGradientColorType--) | Belirtilen dolgu için geçiş renk tipini döndürür. |
| [getGradientDegree()](#getGradientDegree--) | Belirtilen dolgu için geçiş derecesini döndürür. |
| [getGradientFill()](#getGradientFill--) | Alır [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) nesnesini. |
| [getGradientStyle()](#getGradientStyle--) | Belirtilen dolgu için geçiş stilini döndürür. |
| [getGradientVariant()](#getGradientVariant--) | Belirtilen dolgu için geçiş varyantını döndürür. |
| [getImageData()](#getImageData--) | Resim veri bilgisini alır. |
| [getPattern()](#getPattern--) | Bir alanın görüntü desenini temsil eder. |
| [getPatternFill()](#getPatternFill--) | Alır [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) nesnesini. |
| [getPictureFormatType()](#getPictureFormatType--) | Resim formatı tipini alır. |
| [getPresetColor()](#getPresetColor--) | Belirtilen dolgu için geçiş ön ayar rengini döndürür. |
| [getScale()](#getScale--) | Resim formatı ölçeğini alır. |
| [getSetType()](#getSetType--) | Dolgu formatı ayar tipini alır. |
| [getSolidFill()](#getSolidFill--) | Alır [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) nesnesini. |
| [getTexture()](#getTexture--) | Belirtilen dolgu için doku tipini temsil eder. |
| [getTextureFill()](#getTextureFill--) | Alır [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) nesnesini. |
| [getTransparency()](#getTransparency--) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [getType()](#getType--) | Dolgu tipini alır. |
| [hashCode()](#hashCode--) | Karma kodunu alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | Dolgu tipini ayarlar |
| [setImageData(byte[] value)](#setImageData-byte---) | Resim veri bilgisini ayarlar. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Belirtilen dolguyu tek renkli bir degradeye ayarlar. |
| [setPattern(int value)](#setPattern-int-) | Bir alanın görüntü desenini temsil eder. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Resim formatı türünü ayarlar. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Belirtilen dolguyu ön ayarlı renk geçişine ayarlar. |
| [setScale(double value)](#setScale-double-) | Resim formatı ölçeğini ayarlar. |
| [setSetType(int value)](#setSetType-int-) | Dolgu formatı ayar tipini alır. |
| [setTexture(int value)](#setTexture-int-) | Belirtilen dolgu için doku tipini temsil eder. |
| [setTransparency(double value)](#setTransparency-double-) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
| [setType(int value)](#setType-int-) | Doldurma tipini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFillType() {#getFillType--}
```
public int getFillType()
```


Dolgu tipini alır

Bakın [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Belirtilen dolgu için geçiş rengi 1'i döndürür.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Belirtilen dolgu için geçiş rengi 2'yi döndürür.

**Remarks**

Yalnızca degrade renk tipi GradientColorType.TwoColors olduğunda, bu özellik anlamlıdır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Belirtilen dolgu için geçiş renk tipini döndürür.

Bakın [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Belirtilen doldurma için degrade derecesini döndürür. Yalnızca Excel 2007 için geçerlidir.

**Remarks**

Yalnızca 0.0 (koyu) ile 1.0 (açık) arasında bir değer olabilir.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Alır [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) nesnesini.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Belirtilen dolgu için geçiş stilini döndürür.

Bak [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Belirtilen doldurma için degrade varyantını döndürür. Yalnızca Excel 2007 için geçerlidir.

**Remarks**

Yalnızca 1 ile 4 arasında bir değer olabilir; bu değer, Doldurma Efektleri iletişim kutusundaki Degrade sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Resim veri bilgisini alır.

**Remarks**

Doldurma biçimi özel doku biçimi değilse, null döndürür.

**Returns:**
byte[]
### getPattern() {#getPattern--}
```
public int getPattern()
```


Bir alanın görüntü desenini temsil eder.

[FillPattern](../../com.aspose.cells/fillpattern) öğesine bakın.

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Alır [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) nesnesini.

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Resim formatı tipini alır.

Bak [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Belirtilen dolgu için geçiş ön ayar rengini döndürür.

Bakın [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Resim formatı ölçeğini alır.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Dolgu formatı ayar tipini alır.

Bakın [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Alır [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) nesnesini.

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Belirtilen dolgu için doku tipini temsil eder.

Bakınız [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Alır [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) nesnesini.

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Dolgu tipini alır.

Bakın [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Karma kodunu alır.

**Returns:**
int -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


Dolgu tipini ayarlar

Bakın [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Resim veri bilgisini ayarlar.

**Remarks**

Doldurma biçimi özel doku biçimi değilse, null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Belirtilen doldurmayı tek renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| derece | double | Degrade derecesi. 0.0 (karanlık) ile 1.0 (açık) arasında bir değer olabilir. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Bir alanın görüntü desenini temsil eder.

[FillPattern](../../com.aspose.cells/fillpattern) öğesine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Resim formatı türünü ayarlar.

Bak [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Belirtilen doldurmayı önceden tanımlı renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Önceden tanımlı renk tipi |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Resim formatı ölçeğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Dolgu formatı ayar tipini alır.

Bakın [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Belirtilen dolgu için doku tipini temsil eder.

Bakınız [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Belirtilen doldurmayı iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| color2 | [Color](../../com.aspose.cells/color) | İki degrade rengi. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Belirtilen doldurmayı iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| transparency1 | double | color1'in şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
| color2 | [Color](../../com.aspose.cells/color) | İki degrade rengi. |
| transparency2 | double | color2'nin şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Doldurma tipini ayarlar.

Bakın [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

