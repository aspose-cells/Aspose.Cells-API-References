---
title: "TextBoxActiveXControl"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir metin kutusu ActiveX denetimini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Bir metin kutusu ActiveX denetimini temsil eder.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a TextBoxActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50);
         TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Arka planın ole rengini alır. |
| [getBorderOleColor()](#getBorderOleColor--) | Arka planın ole rengini alır. |
| [getBorderStyle()](#getBorderStyle--) | Denetim tarafından kullanılan kenarlık tipini alır. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Denetimin ikili verilerini alır. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Açılır düğmede görüntülenen sembolü belirtir |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Denetime girildiğinde seçim davranışını belirtir. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | ENTER tuşunun davranışını belirtir. |
| [getFont()](#getFont--) | Denetimin yazı tipini temsil eder. |
| [getForeOleColor()](#getForeOleColor--) | Ön planın OLE rengini alır. |
| [getHeight()](#getHeight--) | Denetimin yüksekliğini nokta biriminde alır. |
| [getHideSelection()](#getHideSelection--) | Denetimin odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir. |
| [getIMEMode()](#getIMEMode--) | Denetim odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zamanını alır. |
| [getIntegralHeight()](#getIntegralHeight--) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini belirtir. |
| [getLinkedCell()](#getLinkedCell--) | Bağlı hücreyi alır. |
| [getListFillRange()](#getListFillRange--) | Liste doldurma aralığını alır. |
| [getMaxLength()](#getMaxLength--) | Maksimum karakter sayısını alır |
| [getMouseIcon()](#getMouseIcon--) | Denetim için fare imleci olarak gösterilecek özel bir simgeyi alır. |
| [getMousePointer()](#getMousePointer--) | Denetim için fare imleci olarak gösterilen simge türünü alır. |
| [getPasswordChar()](#getPasswordChar--) | Girilen karakterlerin yerine gösterilecek bir karakter alır. |
| [getScrollBars()](#getScrollBars--) | Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir. |
| [getShadow()](#getShadow--) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Açılır düğmede görüntülenen sembolü belirtir |
| [getSpecialEffect()](#getSpecialEffect--) | Denetimin özel etkisini alır. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Denetimin metninde sekme karakterlerine izin verilip verilmediğini belirtir. |
| [getText()](#getText--) | Denetimin metnini alır. |
| [getTextAlign()](#getTextAlign--) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [getType()](#getType--) | ActiveX denetiminin türünü alır. |
| [getWidth()](#getWidth--) | Denetimin genişliğini puan biriminde alır. |
| [getWorkbook()](#getWorkbook--) | Alır [getWorkbook()](../../com.aspose.cells/activexcontrolbase\\#getWorkbook--) nesnesini. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [isAutoTab()](#isAutoTab--) | Kullanıcı maksimum karakter sayısına ulaştığında odak noktasının otomatik olarak bir sonraki denetime geçip geçmeyeceğini belirtir. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Bir seçimi genişletmek için kullanılan temel birimi belirtir. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Denetim için sürükle ve bırakın etkinleştirilip etkinleştirilmediğini gösterir. |
| [isEditable()](#isEditable--) | Kullanıcının denetime yazıp yazamayacağını gösterir. |
| [isEnabled()](#isEnabled--) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [isLocked()](#isLocked--) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [isMultiLine()](#isMultiLine--) | Denetimin birden fazla satır metin görüntüleyip görüntüleyemeyeceğini belirtir. |
| [isTransparent()](#isTransparent--) | Denetimin şeffaf olup olmadığını gösterir. |
| [isVisible()](#isVisible--) | Bu denetimin görünür olup olmadığını gösterir. |
| [isWordWrapped()](#isWordWrapped--) | Denetimin içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | Kullanıcı maksimum karakter sayısına ulaştığında odak noktasının otomatik olarak bir sonraki denetime geçip geçmeyeceğini belirtir. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Bir seçimi genişletmek için kullanılan temel birimi belirtir. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Arka planın ole rengini ayarlar. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Arka planın ole rengini ayarlar. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Denetim tarafından kullanılan kenarlık tipini ayarlar. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Denetim için sürükle ve bırakın etkinleştirilip etkinleştirilmediğini gösterir. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Açılır düğmede görüntülenen sembolü belirtir |
| [setEditable(boolean value)](#setEditable-boolean-) | Kullanıcının denetime yazıp yazamayacağını gösterir. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Denetime girildiğinde seçim davranışını belirtir. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | ENTER tuşunun davranışını belirtir. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ön planın ole rengini ayarlar. |
| [setHeight(double value)](#setHeight-double-) | Denetimin yüksekliğini puan biriminde ayarlar. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Denetimin odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir. |
| [setIMEMode(int value)](#setIMEMode-int-) | Denetim odağı aldığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modunu ayarlar. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini belirtir. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Bağlantılı hücreyi ayarlar. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Liste doldurma aralığını ayarlar. |
| [setLocked(boolean value)](#setLocked-boolean-) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [setMaxLength(int value)](#setMaxLength-int-) | Maksimum karakter sayısını ayarlar |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Denetim için fare imlecinde gösterilecek özel bir simge ayarlar. |
| [setMousePointer(int value)](#setMousePointer-int-) | Denetim için fare imlecinde gösterilen simge tipini ayarlar. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | Denetimin birden fazla satır metin görüntüleyip görüntüleyemeyeceğini belirtir. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | Girilen karakterlerin yerine gösterilecek bir karakter ayarlar. |
| [setScrollBars(int value)](#setScrollBars-int-) | Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Açılır düğmede görüntülenen sembolü belirtir |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Denetimin özel etkisini ayarlar. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | Denetimin metninde sekme karakterlerine izin verilip verilmediğini belirtir. |
| [setText(String value)](#setText-java.lang.String-) | Denetimin metnini ayarlar. |
| [setTextAlign(int value)](#setTextAlign-int-) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Denetimin şeffaf olup olmadığını gösterir. |
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

**Example**

```
         //excel default color system 12 or green(0x0000FF00)
         activeXControl.setBorderOleColor(/*unchecked*/((int)0x80000012L));
```

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Denetim tarafından kullanılan kenarlık tipini alır.

Bkz [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Example**

```
         activeXControl.setBorderStyle(com.aspose.cells.ControlBorderType.SINGLE);
```

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
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Açılır düğmede görüntülenen sembolü belirtir

Bkz [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Example**

```
         activeXControl.setDropButtonStyle(com.aspose.cells.DropButtonStyle.ARROW);
```

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Denetime girildiğinde seçim davranışını belirtir. True, seçimin denetim son kez etkin olduğunda olduğu gibi değişmeden kalacağını belirtir. False, denetime girildiğinde denetimdeki tüm metnin seçileceğini belirtir.

**Example**

```
         if(!activeXControl.getEnterFieldBehavior())
         {
             activeXControl.setEnterFieldBehavior(true);
         }
```

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


ENTER tuşunun davranışını belirtir. True, ENTER tuşuna basıldığında yeni bir satır oluşturulacağını belirtir. False, ENTER tuşuna basıldığında odak noktasının sekme sırasındaki bir sonraki nesneye taşınacağını belirtir.

**Example**

```
         if(!activeXControl.getEnterKeyBehavior())
         {
             activeXControl.setEnterKeyBehavior(true);
         }
```

**Returns:**
boolean
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
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Denetimin odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir.

**Example**

```
         if(!activeXControl.getHideSelection())
         {
             activeXControl.setHideSelection(true);
         }
```

**Returns:**
boolean
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

**Example**

```
         if(!activeXControl.getIntegralHeight())
         {
             activeXControl.setIntegralHeight(true);
         }
```

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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Maksimum karakter sayısını alır

**Example**

```
         if(activeXControl.getMaxLength() == 0)
         {
             activeXControl.setMaxLength(30);
         }
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
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Girilen karakterlerin yerine gösterilecek bir karakter alır.

**Example**

```
         activeXControl.setPasswordChar('a');
```

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir.

Bakınız [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Example**

```
         activeXControl.setScrollBars(com.aspose.cells.ControlScrollBarType.BARS_VERTICAL);
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
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Açılır düğmede görüntülenen sembolü belirtir

Bkz [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Example**

```
         activeXControl.setShowDropButtonTypeWhen(com.aspose.cells.ShowDropButtonType.FOCUS);
```

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Denetimin özel etkisini alır.

Bkz [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
```

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


Denetimin metninde sekme karakterlerine izin verilip verilmediğini belirtir.

**Example**

```
         if(!activeXControl.getTabKeyBehavior())
         {
             activeXControl.setTabKeyBehavior(true);
         }
```

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Denetimin metnini alır.

**Example**

```
         activeXControl.setText("This is a test.");
```

**Returns:**
java.lang.String
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
         /*Aspose.Cells.Drawing.ActiveXControls.ControlType*/int type = activeXControl.getType();
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
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


Kullanıcı maksimum karakter sayısına ulaştığında odak noktasının otomatik olarak bir sonraki denetime geçip geçmeyeceğini belirtir.

**Example**

```
         if(!activeXControl.isAutoTab())
         {
             activeXControl.setAutoTab(true);
         }
```

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Bir seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin bütün bir kelime olduğunu belirtir.

**Example**

```
         if(!activeXControl.isAutoWordSelected())
         {
             activeXControl.setAutoWordSelected(true);
         }
```

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Denetim için sürükle ve bırakın etkinleştirilip etkinleştirilmediğini gösterir.

**Example**

```
         if(!activeXControl.isDragBehaviorEnabled())
         {
             activeXControl.setDragBehaviorEnabled(true);
         }
```

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Kullanıcının denetime yazıp yazamayacağını gösterir.

**Example**

```
         if(!activeXControl.isEditable())
         {
             activeXControl.setEditable(true);
         }
```

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
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


Denetimin birden fazla satır metin görüntüleyip görüntüleyemeyeceğini belirtir.

**Example**

```
         if(!activeXControl.isMultiLine())
         {
             activeXControl.setMultiLine(true);
         }
```

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
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Denetimin içeriğinin satır sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir.

**Example**

```
         if(!activeXControl.isWordWrapped())
         {
             activeXControl.setWordWrapped(true);
         }
```

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

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


Kullanıcı maksimum karakter sayısına ulaştığında odak noktasının otomatik olarak bir sonraki denetime geçip geçmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Bir seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin bütün bir kelime olduğunu belirtir.

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

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Denetim için sürükle ve bırakın etkinleştirilip etkinleştirilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Açılır düğmede görüntülenen sembolü belirtir

Bkz [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Kullanıcının denetime yazıp yazamayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Denetime girildiğinde seçim davranışını belirtir. True, seçimin denetim son kez etkin olduğunda olduğu gibi değişmeden kalacağını belirtir. False, denetime girildiğinde denetimdeki tüm metnin seçileceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


ENTER tuşunun davranışını belirtir. True, ENTER tuşuna basıldığında yeni bir satır oluşturulacağını belirtir. False, ENTER tuşuna basıldığında odak noktasının sekme sırasındaki bir sonraki nesneye taşınacağını belirtir.

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

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Denetimin odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Maksimum karakter sayısını ayarlar

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

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


Denetimin birden fazla satır metin görüntüleyip görüntüleyemeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


Girilen karakterlerin yerine gösterilecek bir karakter ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

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

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Gölgenin gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Açılır düğmede görüntülenen sembolü belirtir

Bkz [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


Denetimin metninde sekme karakterlerine izin verilip verilmediğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Denetimin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

