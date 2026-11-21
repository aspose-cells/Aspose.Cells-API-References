---
title: "CheckBoxActiveXControl"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir CheckBox ActiveX denetimini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/checkboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class CheckBoxActiveXControl extends ActiveXControl
```

Bir CheckBox ActiveX denetimini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccelerator()](#getAccelerator--) | Denetim için hızlandırıcı tuşu alır. |
| [getAlignment()](#getAlignment--) | Altyazının denetime göre konumunu alır. |
| [getBackOleColor()](#getBackOleColor--) | Arka planın ole rengini alır. |
| [getCaption()](#getCaption--) | Denetim üzerinde görünen açıklayıcı metni alır. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Denetimin ikili verilerini alır. |
| [getFont()](#getFont--) | Denetimin yazı tipini temsil eder. |
| [getForeOleColor()](#getForeOleColor--) | Ön planın OLE rengini alır. |
| [getGroupName()](#getGroupName--) | Grubun adını alır. |
| [getHeight()](#getHeight--) | Denetimin yüksekliğini nokta biriminde alır. |
| [getIMEMode()](#getIMEMode--) | Denetim odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zamanını alır. |
| [getLinkedCell()](#getLinkedCell--) | Bağlı hücreyi alır. |
| [getListFillRange()](#getListFillRange--) | Liste doldurma aralığını alır. |
| [getMouseIcon()](#getMouseIcon--) | Denetim için fare imleci olarak gösterilecek özel bir simgeyi alır. |
| [getMousePointer()](#getMousePointer--) | Denetim için fare imleci olarak gösterilen simge türünü alır. |
| [getPicture()](#getPicture--) | Resmin verisini alır. |
| [getPicturePosition()](#getPicturePosition--) | Denetimin resminin altyazıya göre konumunu alır. |
| [getShadow()](#getShadow--) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [getSpecialEffect()](#getSpecialEffect--) | Denetimin özel etkisini alır. |
| [getTextAlign()](#getTextAlign--) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [getType()](#getType--) | ActiveX denetiminin türünü alır. |
| [getValue()](#getValue--) | Denetimin işaretli olup olmadığını gösterir. |
| [getWidth()](#getWidth--) | Denetimin genişliğini puan biriminde alır. |
| [getWorkbook()](#getWorkbook--) | Alır [getWorkbook()](../../com.aspose.cells/activexcontrolbase\\#getWorkbook--) nesnesini. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [isEnabled()](#isEnabled--) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [isLocked()](#isLocked--) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [isTransparent()](#isTransparent--) | Denetimin şeffaf olup olmadığını gösterir. |
| [isTripleState()](#isTripleState--) | Belirtilen denetimin Null değerleri nasıl göstereceğini belirtir. |
| [isVisible()](#isVisible--) | Bu denetimin görünür olup olmadığını gösterir. |
| [isWordWrapped()](#isWordWrapped--) | Denetimin içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccelerator(char value)](#setAccelerator-char-) | Denetim için hızlandırıcı tuşunu ayarlar. |
| [setAlignment(int value)](#setAlignment-int-) | Altyazının denetime göre konumunu ayarlar. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Arka planın ole rengini ayarlar. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Denetim üzerinde görünen açıklayıcı metni ayarlar. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ön planın ole rengini ayarlar. |
| [setGroupName(String value)](#setGroupName-java.lang.String-) | Grubun adını ayarlar. |
| [setHeight(double value)](#setHeight-double-) | Denetimin yüksekliğini puan biriminde ayarlar. |
| [setIMEMode(int value)](#setIMEMode-int-) | Denetim odağı aldığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modunu ayarlar. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Bağlantılı hücreyi ayarlar. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Liste doldurma aralığını ayarlar. |
| [setLocked(boolean value)](#setLocked-boolean-) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Denetim için fare imlecinde gösterilecek özel bir simge ayarlar. |
| [setMousePointer(int value)](#setMousePointer-int-) | Denetim için fare imlecinde gösterilen simge tipini ayarlar. |
| [setPicture(byte[] value)](#setPicture-byte---) | Resmin verisini ayarlar. |
| [setPicturePosition(int value)](#setPicturePosition-int-) | Denetimin resminin altyazıya göre konumunu ayarlar. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Denetimin özel etkisini ayarlar. |
| [setTextAlign(int value)](#setTextAlign-int-) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Denetimin şeffaf olup olmadığını gösterir. |
| [setTripleState(boolean value)](#setTripleState-boolean-) | Belirtilen denetimin Null değerleri nasıl göstereceğini belirtir. |
| [setValue(int value)](#setValue-int-) | Denetimin işaretli olup olmadığını gösterir. |
| [setVisible(boolean value)](#setVisible-boolean-) | Bu denetimin görünür olup olmadığını gösterir. |
| [setWidth(double value)](#setWidth-double-) | Denetimin genişliğini puan biriminde ayarlar. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Denetimin içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir. |
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
### getAccelerator() {#getAccelerator--}
```
public char getAccelerator()
```


Denetim için hızlandırıcı tuşu alır.

**Returns:**
char
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Altyazının denetime göre konumunu alır.

Bkz [ControlCaptionAlignmentType](../../com.aspose.cells/controlcaptionalignmenttype).

**Returns:**
int
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Arka planın ole rengini alır.

**Returns:**
int
### getCaption() {#getCaption--}
```
public String getCaption()
```


Denetim üzerinde görünen açıklayıcı metni alır.

**Returns:**
java.lang.String
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
### getGroupName() {#getGroupName--}
```
public String getGroupName()
```


Grubun adını alır.

**Returns:**
java.lang.String
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
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


Resmin verisini alır.

**Returns:**
byte[]
### getPicturePosition() {#getPicturePosition--}
```
public int getPicturePosition()
```


Denetimin resminin altyazıya göre konumunu alır.

Bkz [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Gölgenin gösterilip gösterilmeyeceğini belirtir.

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
public int getValue()
```


Denetimin işaretli olup olmadığını gösterir.

Bkz [CheckValueType](../../com.aspose.cells/checkvaluetype).

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
### isTripleState() {#isTripleState--}
```
public boolean isTripleState()
```


Belirtilen denetimin Null değerleri nasıl göstereceğini belirtir.

**Remarks**

| Ayar | Açıklama |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Doğru | Denetim, Evet, Hayır ve Null değerleri için durumlar arasında dönecektir. Değer özelliği Null olarak ayarlandığında denetim karartılmış (gri) görünür. |
| Yanlış | (Default) Kontrol, Evet ve Hayır değerleri için durumlar arasında dönecektir. Null değerler, Hayır değerleri gibi gösterilir. |

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Bu denetimin görünür olup olmadığını gösterir.

**Returns:**
boolean
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Denetimin içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir.

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




### setAccelerator(char value) {#setAccelerator-char-}
```
public void setAccelerator(char value)
```


Denetim için hızlandırıcı tuşunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Altyazının denetime göre konumunu ayarlar.

Bkz [ControlCaptionAlignmentType](../../com.aspose.cells/controlcaptionalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Denetim üzerinde görünen açıklayıcı metni ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

### setGroupName(String value) {#setGroupName-java.lang.String-}
```
public void setGroupName(String value)
```


Grubun adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


Resmin verisini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setPicturePosition(int value) {#setPicturePosition-int-}
```
public void setPicturePosition(int value)
```


Denetimin resminin altyazıya göre konumunu ayarlar.

Bkz [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Denetimin şeffaf olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTripleState(boolean value) {#setTripleState-boolean-}
```
public void setTripleState(boolean value)
```


Belirtilen denetimin Null değerleri nasıl göstereceğini belirtir.

**Remarks**

| Ayar | Açıklama |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Doğru | Denetim, Evet, Hayır ve Null değerleri için durumlar arasında dönecektir. Değer özelliği Null olarak ayarlandığında denetim karartılmış (gri) görünür. |
| Yanlış | (Default) Kontrol, Evet ve Hayır değerleri için durumlar arasında dönecektir. Null değerler, Hayır değerleri gibi gösterilir. |

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setValue(int value) {#setValue-int-}
```
public void setValue(int value)
```


Denetimin işaretli olup olmadığını gösterir.

Bkz [CheckValueType](../../com.aspose.cells/checkvaluetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Denetimin içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

