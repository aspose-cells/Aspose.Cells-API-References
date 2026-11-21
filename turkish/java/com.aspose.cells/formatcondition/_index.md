---
title: "FormatCondition"
second_title: "Aspose.Cells for Java API Referansı"
description: "Koşullu biçimlendirme koşulunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Koşullu biçimlendirme koşulunu temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
 
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
 
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
 
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         //Saving the Excel file
         workbook.save("output.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Koşullu biçimlendirme "AboveAverage" örneğini al. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Koşullu biçimlendirme "ColorScale" örneğini al. |
| [getDataBar()](#getDataBar--) | Koşullu biçimlendirme "DataBar" örneğini al. |
| [getFormula1()](#getFormula1--) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Bu biçim koşulu ile ilişkili değeri veya ifadeyi alır. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Hücrenin koşullu biçimlendirmesinin formülünü alır. |
| [getFormula2()](#getFormula2--) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Bu biçim koşulu ile ilişkili değeri veya ifadeyi alır. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Hücrenin koşullu biçimlendirmesinin formülünü alır. |
| [getIconSet()](#getIconSet--) | Koşullu biçimlendirme "IconSet" örneğini al. |
| [getOperator()](#getOperator--) | Koşullu biçimlendirme operatör tipini alır. |
| [getPriority()](#getPriority--) | Bu koşullu biçimlendirme kuralının önceliği. |
| [getStopIfTrue()](#getStopIfTrue--) | Doğru, daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz, bu kural doğru olarak değerlendirildiğinde. |
| [getStyle()](#getStyle--) | Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar. |
| [getText()](#getText--) | \"metin içerir\" koşullu biçimlendirme kuralındaki metin değeri. |
| [getTimePeriod()](#getTimePeriod--) | \"date occurrin\" koşullu biçimlendirme kuralındaki geçerli zaman dilimi. |
| [getTop10()](#getTop10--) | Koşullu biçimlendirmenin \"Top10\" örneğini al. |
| [getType()](#getType--) | Koşullu biçim Türünün durumunu alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi ayarlar. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Bu biçim koşulu ile ilişkili değeri veya ifadeyi ayarlar. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi ayarlar. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Bu biçim koşulu ile ilişkili değeri veya ifadeyi ayarlar. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Bu biçim koşulu ile ilişkili değeri veya ifadeyi ayarlar. |
| [setOperator(int value)](#setOperator-int-) | Koşullu biçim operatör tipini ayarlar. |
| [setPriority(int value)](#setPriority-int-) | Bu koşullu biçimlendirme kuralının önceliği. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | Doğru, daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz, bu kural doğru olarak değerlendirildiğinde. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar. |
| [setText(String value)](#setText-java.lang.String-) | \"metin içerir\" koşullu biçimlendirme kuralındaki metin değeri. |
| [setTimePeriod(int value)](#setTimePeriod-int-) | \"date occurrin\" koşullu biçimlendirme kuralındaki geçerli zaman dilimi. |
| [setType(int value)](#setType-int-) | Koşullu biçim Türünün olup olmadığını ayarlar. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Koşullu biçimlendirmenin \"AboveAverage\" örneğini al. Varsayılan örnek, aralıktaki tüm değerlerin ortalamasının üzerindeki hücreleri vurgulayan bir kuraldır. Yalnızca type = AboveAverage için geçerlidir.

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


Koşullu biçimlendirmenin \"ColorScale\" örneğini al. Varsayılan örnek, \"yeşil-sarı-kırmızı\" 3RenkÖlçeği'dir. Yalnızca type = ColorScale için geçerlidir.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Koşullu biçimlendirmenin \"DataBar\" örneğini al. Varsayılan örneğin rengi mavidir. Yalnızca type = DataBar için geçerlidir.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır.

**Remarks**

Formül ayarlamadan önce lütfen tüm alanları ekleyin. Bu koşul için formül ayarlarken, giriş değeri '=' ile başlıyorsa formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak alınır. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\\\"=...\\\"".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Bu biçim koşulu ile ilişkili değeri veya ifadeyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Bu biçim koşulu ile ilişkili değer veya ifade.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır.

**Remarks**

Verilen hücre bu koşullu biçimlendirme içinde olmalıdır, aksi takdirde null döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Hücrenin koşullu biçimlendirmesi ile ilişkili değer veya ifade.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Hücrenin koşullu biçimlendirmesinin formülünü alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Formül.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır.

**Remarks**

Formül ayarlamadan önce lütfen tüm alanları ekleyin. Bu koşul için formül ayarlarken, giriş değeri '=' ile başlıyorsa formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak alınır. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\\\"=...\\\"".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Bu biçim koşulu ile ilişkili değeri veya ifadeyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Bu biçim koşulu ile ilişkili değer veya ifade.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır.

**Remarks**

Verilen hücre bu koşullu biçimlendirme içinde olmalıdır, aksi takdirde null döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Hücrenin koşullu biçimlendirmesi ile ilişkili değer veya ifade.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Hücrenin koşullu biçimlendirmesinin formülünü alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Formül.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Koşullu biçimlendirmenin \"IconSet\" örneğini al. Varsayılan örneğin IconSetType'ı TrafficLights31'dir. Yalnızca type = IconSet için geçerlidir.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Koşullu biçimlendirme operatör tipini alır.

Bakınız [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


Bu koşullu biçimlendirme kuralının önceliği. Bu değer, hangi biçimin değerlendirileceğini ve işleneceğini belirlemek için kullanılır. Daha düşük sayısal değerler, daha yüksek sayısal değerlerden daha yüksek önceliğe sahiptir; '1' en yüksek önceliktir.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


Doğru, daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz, bu kural doğru olarak değerlendirildiğinde. Yalnızca Excel 2007 için geçerlidir;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


\"metin içerir\" koşullu biçimlendirme kuralındaki metin değeri. Yalnızca type = containsText, notContainsText, beginsWith ve endsWith için geçerlidir. Varsayılan değer null'dur.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


\"date occurrin\" koşullu biçimlendirme kuralındaki geçerli zaman dilimi. Yalnızca type = timePeriod için geçerlidir. Varsayılan değer TimePeriodType.Today'dir.

[TimePeriodType](../../com.aspose.cells/timeperiodtype) adresine bakın.

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Koşullu biçimlendirmenin \"Top10\" örneğini al. Varsayılan örnek, değerleri en üst 10 dilim içinde olan hücreleri vurgulayan bir kuraldır. Yalnızca type = Top10 için geçerlidir.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Koşullu biçim Türünün durumunu alır.

Bak [FormatConditionType](../../com.aspose.cells/formatconditiontype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi ayarlar.

**Remarks**

Formül ayarlamadan önce lütfen tüm alanları ekleyin. Bu koşul için formül ayarlarken, giriş değeri '=' ile başlıyorsa formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak alınır. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\\\"=...\\\"".

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Bu biçim koşulu ile ilişkili değeri veya ifadeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Bu format koşuluyla ilişkili değer veya ifade. Giriş değeri '=' ile başlıyorsa, formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak kabul edilir. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\\"=...\\"". |
| isR1C1 | boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi ayarlar.

**Remarks**

Formül ayarlamadan önce lütfen tüm alanları ekleyin. Bu koşul için formül ayarlarken, giriş değeri '=' ile başlıyorsa formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak alınır. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\\\"=...\\\"".

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Bu biçim koşulu ile ilişkili değeri veya ifadeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Bu format koşuluyla ilişkili değer veya ifade. Giriş değeri '=' ile başlıyorsa, formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak kabul edilir. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\\"=...\\"". |
| isR1C1 | boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Bu biçim koşulu ile ilişkili değeri veya ifadeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula1 | java.lang.String | Bu format koşuluyla ilişkili değer veya ifade. Giriş değeri '=' ile başlıyorsa, formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak kabul edilir. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\\"=...\\"". |
| formula2 | java.lang.String | Bu format koşuluyla ilişkili değer veya ifade. Giriş formatı formula1 ile aynıdır. |
| isR1C1 | boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Koşullu biçim operatör tipini ayarlar.

Bakınız [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


Bu koşullu biçimlendirme kuralının önceliği. Bu değer, hangi biçimin değerlendirileceğini ve işleneceğini belirlemek için kullanılır. Daha düşük sayısal değerler, daha yüksek sayısal değerlerden daha yüksek önceliğe sahiptir; '1' en yüksek önceliktir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


Doğru, daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz, bu kural doğru olarak değerlendirildiğinde. Yalnızca Excel 2007 için geçerlidir;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


\"metin içerir\" koşullu biçimlendirme kuralındaki metin değeri. Yalnızca type = containsText, notContainsText, beginsWith ve endsWith için geçerlidir. Varsayılan değer null'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


\"date occurrin\" koşullu biçimlendirme kuralındaki geçerli zaman dilimi. Yalnızca type = timePeriod için geçerlidir. Varsayılan değer TimePeriodType.Today'dir.

[TimePeriodType](../../com.aspose.cells/timeperiodtype) adresine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Koşullu biçim Türünün olup olmadığını ayarlar.

Bak [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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

