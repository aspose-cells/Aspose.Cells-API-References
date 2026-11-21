---
title: "SpinButtonActiveXControl"
second_title: "Aspose.Cells for Java API Referansı"
description: "SpinButton kontrolünü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/spinbuttonactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class SpinButtonActiveXControl extends ActiveXControl
```

SpinButton kontrolünü temsil eder.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a ToggleButtonActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50);
         SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Arka planın ole rengini alır. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Denetimin ikili verilerini alır. |
| [getFont()](#getFont--) | Denetimin yazı tipini temsil eder. |
| [getForeOleColor()](#getForeOleColor--) | Ön planın OLE rengini alır. |
| [getHeight()](#getHeight--) | Denetimin yüksekliğini nokta biriminde alır. |
| [getIMEMode()](#getIMEMode--) | Denetim odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zamanını alır. |
| [getLinkedCell()](#getLinkedCell--) | Bağlı hücreyi alır. |
| [getListFillRange()](#getListFillRange--) | Liste doldurma aralığını alır. |
| [getMax()](#getMax--) | Maksimum kabul edilebilir değeri alır. |
| [getMin()](#getMin--) | Minimum kabul edilebilir değeri alır. |
| [getMouseIcon()](#getMouseIcon--) | Denetim için fare imleci olarak gösterilecek özel bir simgeyi alır. |
| [getMousePointer()](#getMousePointer--) | Denetim için fare imleci olarak gösterilen simge türünü alır. |
| [getOrientation()](#getOrientation--) | SpinButton veya ScrollBar'ın dikey mi yoksa yatay mı yönlendirildiğini alır. |
| [getPosition()](#getPosition--) | Değeri alır. |
| [getShadow()](#getShadow--) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [getSmallChange()](#getSmallChange--) | Position özelliğinin değiştiği miktarı alır |
| [getTextAlign()](#getTextAlign--) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [getType()](#getType--) | ActiveX denetiminin türünü alır. |
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
| [setEnabled(boolean value)](#setEnabled-boolean-) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ön planın ole rengini ayarlar. |
| [setHeight(double value)](#setHeight-double-) | Denetimin yüksekliğini puan biriminde ayarlar. |
| [setIMEMode(int value)](#setIMEMode-int-) | Denetim odağı aldığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modunu ayarlar. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Bağlantılı hücreyi ayarlar. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Liste doldurma aralığını ayarlar. |
| [setLocked(boolean value)](#setLocked-boolean-) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [setMax(int value)](#setMax-int-) | Maksimum kabul edilebilir değeri ayarlar. |
| [setMin(int value)](#setMin-int-) | Minimum kabul edilebilir değeri ayarlar. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Denetim için fare imlecinde gösterilecek özel bir simge ayarlar. |
| [setMousePointer(int value)](#setMousePointer-int-) | Denetim için fare imlecinde gösterilen simge tipini ayarlar. |
| [setOrientation(int value)](#setOrientation-int-) | SpinButton veya ScrollBar'ın dikey mi yoksa yatay mı yönlendirileceğini ayarlar. |
| [setPosition(int value)](#setPosition-int-) | Değeri ayarlar. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [setSmallChange(int value)](#setSmallChange-int-) | Position özelliğinin değiştiği miktarı ayarlar |
| [setTextAlign(int value)](#setTextAlign-int-) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Denetimin şeffaf olup olmadığını gösterir. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### getMax() {#getMax--}
```
public int getMax()
```


Maksimum kabul edilebilir değeri alır.

**Example**

```
         activeXControl.setMax(100);
```

**Returns:**
int
### getMin() {#getMin--}
```
public int getMin()
```


Minimum kabul edilebilir değeri alır.

**Example**

```
         activeXControl.setMin(0);
```

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
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


SpinButton veya ScrollBar'ın dikey mi yoksa yatay mı yönlendirildiğini alır.

Bakınız [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).

**Example**

```
         if(activeXControl.getOrientation() == com.aspose.cells.ControlScrollOrientation.AUTO)
         {
             activeXControl.setOrientation(com.aspose.cells.ControlScrollOrientation.HORIZONTAL);
         }
```

**Returns:**
int
### getPosition() {#getPosition--}
```
public int getPosition()
```


Değeri alır.

**Example**

```
         activeXControl.setPosition(30);
```

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Gölgenin gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getSmallChange() {#getSmallChange--}
```
public int getSmallChange()
```


Position özelliğinin değiştiği miktarı alır

**Example**

```
         activeXControl.setSmallChange(5);
```

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
### getType() {#getType--}
```
public int getType()
```


ActiveX denetiminin türünü alır.

Bkz [ControlType](../../com.aspose.cells/controltype).

**Example**

```
         if(activeXControl.getType() == com.aspose.cells.ControlType.SPIN_BUTTON)
         {
             //do something
         }
```

**Returns:**
int
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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMax(int value) {#setMax-int-}
```
public void setMax(int value)
```


Maksimum kabul edilebilir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMin(int value) {#setMin-int-}
```
public void setMin(int value)
```


Minimum kabul edilebilir değeri ayarlar.

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

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


SpinButton veya ScrollBar'ın dikey mi yoksa yatay mı yönlendirileceğini ayarlar.

Bakınız [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Değeri ayarlar.

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

### setSmallChange(int value) {#setSmallChange-int-}
```
public void setSmallChange(int value)
```


Position özelliğinin değiştiği miktarı ayarlar

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Denetimin şeffaf olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

