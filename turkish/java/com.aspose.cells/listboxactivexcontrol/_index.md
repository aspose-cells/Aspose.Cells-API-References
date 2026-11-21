---
title: "ListBoxActiveXControl"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir ListBox ActiveX denetimini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/listboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ListBoxActiveXControl extends ActiveXControl
```

Bir ListBox ActiveX denetimini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Arka planın ole rengini alır. |
| [getBorderOleColor()](#getBorderOleColor--) | Arka planın ole rengini alır. |
| [getBorderStyle()](#getBorderStyle--) | Denetim tarafından kullanılan kenarlık tipini alır. |
| [getBoundColumn()](#getBoundColumn--) | ComboBox veya ListBox için MultiSelect özelliği değeri (fmMultiSelectSingle) olduğunda Value özelliğinin nasıl belirlendiğini temsil eder. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | ComboBox veya ListBox içinde görüntülenecek sütun sayısını temsil eder. |
| [getColumnWidths()](#getColumnWidths--) | Sütunun genişliğini alır. |
| [getData()](#getData--) | Denetimin ikili verilerini alır. |
| [getFont()](#getFont--) | Denetimin yazı tipini temsil eder. |
| [getForeOleColor()](#getForeOleColor--) | Ön planın OLE rengini alır. |
| [getHeight()](#getHeight--) | Denetimin yüksekliğini nokta biriminde alır. |
| [getIMEMode()](#getIMEMode--) | Denetim odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zamanını alır. |
| [getIntegralHeight()](#getIntegralHeight--) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini belirtir. |
| [getLinkedCell()](#getLinkedCell--) | Bağlı hücreyi alır. |
| [getListFillRange()](#getListFillRange--) | Liste doldurma aralığını alır. |
| [getListStyle()](#getListStyle--) | Görsel görünümü alır. |
| [getListWidth()](#getListWidth--) | Genişliği nokta biriminde alır. |
| [getMatchEntry()](#getMatchEntry--) | Bir ListBox veya ComboBox'ın, kullanıcının yazarken listesini nasıl aradığını gösterir. |
| [getMouseIcon()](#getMouseIcon--) | Denetim için fare imleci olarak gösterilecek özel bir simgeyi alır. |
| [getMousePointer()](#getMousePointer--) | Denetim için fare imleci olarak gösterilen simge türünü alır. |
| [getScrollBars()](#getScrollBars--) | Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir. |
| [getSelectionType()](#getSelectionType--) | Denetimin birden fazla seçim yapmasına izin verip vermediğini gösterir. |
| [getShadow()](#getShadow--) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Sütun başlıklarının gösterilip gösterilmediğini belirtir. |
| [getSpecialEffect()](#getSpecialEffect--) | Denetimin özel etkisini alır. |
| [getTextAlign()](#getTextAlign--) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [getTextColumn()](#getTextColumn--) | Kullanıcıya gösterilecek ComboBox veya ListBox içindeki sütunu temsil eder. |
| [getType()](#getType--) | ActiveX denetiminin türünü alır. |
| [getValue()](#getValue--) | Denetimin değerini alır. |
| [getWidth()](#getWidth--) | Denetimin genişliğini puan biriminde alır. |
| [getWorkbook()](#getWorkbook--) | Alır [getWorkbook()](../../com.aspose.cells/activexcontrolbase\\#getWorkbook--) nesnesini. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [isEnabled()](#isEnabled--) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [isLocked()](#isLocked--) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [isTransparent()](#isTransparent--) | Denetimin şeffaf olup olmadığını gösterir. |
| [isVisible()](#isVisible--) | Bu denetimin görünür olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Arka planın ole rengini ayarlar. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Arka planın ole rengini ayarlar. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Denetim tarafından kullanılan kenarlık tipini ayarlar. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | ComboBox veya ListBox için MultiSelect özelliği değeri (fmMultiSelectSingle) olduğunda Value özelliğinin nasıl belirlendiğini temsil eder. |
| [setColumnCount(int value)](#setColumnCount-int-) | ComboBox veya ListBox içinde görüntülenecek sütun sayısını temsil eder. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Sütunun genişliğini ayarlar. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ön planın ole rengini ayarlar. |
| [setHeight(double value)](#setHeight-double-) | Denetimin yüksekliğini puan biriminde ayarlar. |
| [setIMEMode(int value)](#setIMEMode-int-) | Denetim odağı aldığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modunu ayarlar. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini belirtir. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Bağlantılı hücreyi ayarlar. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Liste doldurma aralığını ayarlar. |
| [setListStyle(int value)](#setListStyle-int-) | Görsel görünümü ayarlar. |
| [setListWidth(double value)](#setListWidth-double-) | Genişliği puan biriminde ayarlar. |
| [setLocked(boolean value)](#setLocked-boolean-) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Bir ListBox veya ComboBox'ın, kullanıcının yazarken listesini nasıl aradığını gösterir. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Denetim için fare imlecinde gösterilecek özel bir simge ayarlar. |
| [setMousePointer(int value)](#setMousePointer-int-) | Denetim için fare imlecinde gösterilen simge tipini ayarlar. |
| [setScrollBars(int value)](#setScrollBars-int-) | Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir. |
| [setSelectionType(int value)](#setSelectionType-int-) | Denetimin birden fazla seçim yapmasına izin verip vermediğini gösterir. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Sütun başlıklarının gösterilip gösterilmediğini belirtir. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Denetimin özel etkisini ayarlar. |
| [setTextAlign(int value)](#setTextAlign-int-) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [setTextColumn(int value)](#setTextColumn-int-) | Kullanıcıya gösterilecek ComboBox veya ListBox içindeki sütunu temsil eder. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Denetimin şeffaf olup olmadığını gösterir. |
| [setValue(String value)](#setValue-java.lang.String-) | Denetimin değerini ayarlar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Bu denetimin görünür olup olmadığını gösterir. |
| [setWidth(double value)](#setWidth-double-) | Denetimin genişliğini puan biriminde ayarlar. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Arka planın ole rengini alır.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Arka planın ole rengini alır.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Denetim tarafından kullanılan kenarlık tipini alır.

Bkz [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


ComboBox veya ListBox için MultiSelect özelliği değeri (fmMultiSelectSingle) olduğunda Value özelliğinin nasıl belirlendiğini temsil eder.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


ComboBox veya ListBox içinde görüntülenecek sütun sayısını temsil eder.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Sütunun genişliğini alır.

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


Denetimin ikili verilerini alır.

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


Denetimin yazı tipini temsil eder.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Ön planın OLE rengini alır.

**Remarks**

Görüntü denetimi için geçerli değildir.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Denetimin yüksekliğini nokta biriminde alır.

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Denetim odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zamanını alır.

Bkz [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini belirtir.

**Returns:**
boolean
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Bağlı hücreyi alır.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Liste doldurma aralığını alır.

**Returns:**
java.lang.String
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Görsel görünümü alır.

Bkz [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Genişliği nokta biriminde alır.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Bir ListBox veya ComboBox'ın, kullanıcının yazarken listesini nasıl aradığını gösterir.

Bkz [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Denetim için fare imleci olarak gösterilecek özel bir simgeyi alır.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Denetim için fare imleci olarak gösterilen simge türünü alır.

Bkz [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir.

Bakınız [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Returns:**
int
### getSelectionType() {#getSelectionType--}
```
public int getSelectionType()
```


Denetimin birden fazla seçim yapmasına izin verip vermediğini gösterir.

Bakınız [SelectionType](../../com.aspose.cells/selectiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Gölgenin gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Sütun başlıklarının gösterilip gösterilmediğini belirtir.

**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Denetimin özel etkisini alır.

Bkz [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Kullanıcıya gösterilecek ComboBox veya ListBox içindeki sütunu temsil eder.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


ActiveX denetiminin türünü alır.

Bkz [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


Denetimin değerini alır.

**Remarks**

Yalnızca [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\\#getSelectionType--) SelectionType.Single olduğunda etkili olur;

**Returns:**
java.lang.String
### getWidth() {#getWidth--}
```
public double getWidth()
```


Denetimin genişliğini puan biriminde alır.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Alır [getWorkbook()](../../com.aspose.cells/activexcontrolbase\\#getWorkbook--) nesnesini.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Denetimin şeffaf olup olmadığını gösterir.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Bu denetimin görünür olup olmadığını gösterir.

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Arka planın ole rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Arka planın ole rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Denetim tarafından kullanılan kenarlık tipini ayarlar.

Bkz [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


ComboBox veya ListBox için MultiSelect özelliği değeri (fmMultiSelectSingle) olduğunda Value özelliğinin nasıl belirlendiğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


ComboBox veya ListBox içinde görüntülenecek sütun sayısını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Sütunun genişliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Ön planın ole rengini ayarlar.

**Remarks**

Görüntü denetimi için geçerli değildir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Denetimin yüksekliğini puan biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Denetim odağı aldığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modunu ayarlar.

Bkz [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Bağlantılı hücreyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Liste doldurma aralığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Görsel görünümü ayarlar.

Bkz [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Genişliği puan biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Bir ListBox veya ComboBox'ın, kullanıcının yazarken listesini nasıl aradığını gösterir.

Bkz [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Denetim için fare imlecinde gösterilecek özel bir simge ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Denetim için fare imlecinde gösterilen simge tipini ayarlar.

Bkz [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir.

Bakınız [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSelectionType(int value) {#setSelectionType-int-}
```
public void setSelectionType(int value)
```


Denetimin birden fazla seçim yapmasına izin verip vermediğini gösterir.

Bakınız [SelectionType](../../com.aspose.cells/selectiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Gölgenin gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Sütun başlıklarının gösterilip gösterilmediğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Denetimin özel etkisini ayarlar.

Bkz [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Kullanıcıya gösterilecek ComboBox veya ListBox içindeki sütunu temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Denetimin şeffaf olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Denetimin değerini ayarlar.

**Remarks**

Yalnızca [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\\#getSelectionType--) SelectionType.Single olduğunda etkili olur;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Bu denetimin görünür olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Denetimin genişliğini puan biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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

