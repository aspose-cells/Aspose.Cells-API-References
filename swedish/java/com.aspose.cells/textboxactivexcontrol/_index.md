---
title: "TextBoxActiveXControl"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en textruta‑ActiveX‑kontroll."
type: docs
url: /sv/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Representerar en textruta‑ActiveX‑kontroll.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Hämtar ole-färgen för bakgrunden. |
| [getBorderOleColor()](#getBorderOleColor--) | Hämtar ole-färgen för bakgrunden. |
| [getBorderStyle()](#getBorderStyle--) | Hämtar typen av kant som används av kontrollen. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Hämtar kontrollens binära data. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Anger symbolen som visas på rullknappen |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Anger markeringsbeteende när kontrollen aktiveras. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | Anger beteendet för ENTER-tangenten. |
| [getFont()](#getFont--) | Representerar kontrollens teckensnitt. |
| [getForeOleColor()](#getForeOleColor--) | Hämtar förgrundens OLE-färg. |
| [getHeight()](#getHeight--) | Hämtar kontrollens höjd i punktenheter. |
| [getHideSelection()](#getHideSelection--) | Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus. |
| [getIMEMode()](#getIMEMode--) | Hämtar standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [getIntegralHeight()](#getIntegralHeight--) | Indikerar om kontrollen endast visar kompletta textrader utan att visa några partiella rader. |
| [getLinkedCell()](#getLinkedCell--) | Hämtar den länkade cellen. |
| [getListFillRange()](#getListFillRange--) | Hämtar listans fyllningsintervall. |
| [getMaxLength()](#getMaxLength--) | Hämtar det maximala antalet tecken |
| [getMouseIcon()](#getMouseIcon--) | Hämtar en anpassad ikon som ska visas som muspekare för kontrollen. |
| [getMousePointer()](#getMousePointer--) | Hämtar typen av ikon som visas som muspekare för kontrollen. |
| [getPasswordChar()](#getPasswordChar--) | Hämtar ett tecken som ska visas i stället för de inmatade tecknen. |
| [getScrollBars()](#getScrollBars--) | Indikerar om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen. |
| [getShadow()](#getShadow--) | Indikerar om en skugga ska visas. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Anger symbolen som visas på rullknappen |
| [getSpecialEffect()](#getSpecialEffect--) | Hämtar kontrollens specialeffekt. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Indikerar om tabulatortecken är tillåtna i kontrollens text. |
| [getText()](#getText--) | Hämtar texten för kontrollen. |
| [getTextAlign()](#getTextAlign--) | Representerar hur texten som används av kontrollen ska justeras. |
| [getType()](#getType--) | Hämtar typen av ActiveX-kontrollen. |
| [getWidth()](#getWidth--) | Hämtar bredden på kontrollen i enheten punkter. |
| [getWorkbook()](#getWorkbook--) | Hämtar [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) objektet. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [isAutoTab()](#isAutoTab--) | Anger om fokus automatiskt kommer att flyttas till nästa kontroll när användaren anger det maximala antalet tecken. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Anger den grundläggande enheten som används för att utöka en markering. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Anger om dra och släpp är aktiverat för kontrollen. |
| [isEditable()](#isEditable--) | Anger om användaren kan skriva i kontrollen. |
| [isEnabled()](#isEnabled--) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [isLocked()](#isLocked--) | Anger om data i kontrollen är låst för redigering. |
| [isMultiLine()](#isMultiLine--) | Anger om kontrollen kan visa mer än en rad text. |
| [isTransparent()](#isTransparent--) | Anger om kontrollen är transparent. |
| [isVisible()](#isVisible--) | Anger om den här kontrollen är synlig. |
| [isWordWrapped()](#isWordWrapped--) | Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | Anger om fokus automatiskt kommer att flyttas till nästa kontroll när användaren anger det maximala antalet tecken. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Anger den grundläggande enheten som används för att utöka en markering. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Ställer in typen av ram som används av kontrollen. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Anger om dra och släpp är aktiverat för kontrollen. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Anger symbolen som visas på rullknappen |
| [setEditable(boolean value)](#setEditable-boolean-) | Anger om användaren kan skriva i kontrollen. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Anger markeringsbeteende när kontrollen aktiveras. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | Anger beteendet för ENTER-tangenten. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ställer in OLE-färgen för förgrunden. |
| [setHeight(double value)](#setHeight-double-) | Ställer in höjden på kontrollen i enheten punkter. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus. |
| [setIMEMode(int value)](#setIMEMode-int-) | Ställer in standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indikerar om kontrollen endast visar kompletta textrader utan att visa några partiella rader. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Ställer in den länkade cellen. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Ställer in listfyllningsområdet. |
| [setLocked(boolean value)](#setLocked-boolean-) | Anger om data i kontrollen är låst för redigering. |
| [setMaxLength(int value)](#setMaxLength-int-) | Ställer in maximalt antal tecken |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Ställer in en anpassad ikon som ska visas som muspekare för kontrollen. |
| [setMousePointer(int value)](#setMousePointer-int-) | Ställer in typen av ikon som visas som muspekare för kontrollen. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | Anger om kontrollen kan visa mer än en rad text. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | Ställer in ett tecken som ska visas i stället för de inmatade tecknen. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indikerar om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indikerar om en skugga ska visas. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Anger symbolen som visas på rullknappen |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Ställer in den speciella effekten för kontrollen. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | Indikerar om tabulatortecken är tillåtna i kontrollens text. |
| [setText(String value)](#setText-java.lang.String-) | Ställer in texten för kontrollen. |
| [setTextAlign(int value)](#setTextAlign-int-) | Representerar hur texten som används av kontrollen ska justeras. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Anger om kontrollen är transparent. |
| [setVisible(boolean value)](#setVisible-boolean-) | Anger om den här kontrollen är synlig. |
| [setWidth(double value)](#setWidth-double-) | Ställer in bredden på kontrollen i enheten punkter. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Hämtar ole-färgen för bakgrunden.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Hämtar ole-färgen för bakgrunden.

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


Hämtar typen av kant som används av kontrollen.

Se [ControlBorderType](../../com.aspose.cells/controlbordertype).

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


Hämtar kontrollens binära data.

**Returns:**
byte[]
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Anger symbolen som visas på rullknappen

Se [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

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


Anger urvalsbeteende när kontrollen öppnas. True anger att urvalet förblir oförändrat från senaste gången kontrollen var aktiv. False anger att all text i kontrollen kommer att markeras när kontrollen öppnas.

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


Anger beteendet för ENTER-tangenten. True betyder att tryck på ENTER skapar en ny rad. False betyder att tryck på ENTER flyttar fokus till nästa objekt i tabb-ordningen.

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


Representerar kontrollens teckensnitt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Hämtar förgrundens OLE-färg.

**Remarks**

Gäller inte för bildkontrollen.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Hämtar kontrollens höjd i punktenheter.

**Returns:**
double
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus.

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


Hämtar standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus.

Se [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


Indikerar om kontrollen endast visar kompletta textrader utan att visa några partiella rader.

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


Hämtar den länkade cellen.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Hämtar listans fyllningsintervall.

**Returns:**
java.lang.String
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Hämtar det maximala antalet tecken

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


Hämtar en anpassad ikon som ska visas som muspekare för kontrollen.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Hämtar typen av ikon som visas som muspekare för kontrollen.

Se [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Hämtar ett tecken som ska visas i stället för de inmatade tecknen.

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


Indikerar om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen.

Se [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

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


Indikerar om en skugga ska visas.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Anger symbolen som visas på rullknappen

Se [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

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


Hämtar kontrollens specialeffekt.

Se [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

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


Indikerar om tabulatortecken är tillåtna i kontrollens text.

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


Hämtar texten för kontrollen.

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


Representerar hur texten som används av kontrollen ska justeras.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av ActiveX-kontrollen.

Se [ControlType](../../com.aspose.cells/controltype).

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


Hämtar bredden på kontrollen i enheten punkter.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Hämtar [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) objektet.

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


Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet.

**Returns:**
boolean
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


Anger om fokus automatiskt kommer att flyttas till nästa kontroll när användaren anger det maximala antalet tecken.

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


Anger den grundläggande enheten som används för att utöka ett urval. True anger att den grundläggande enheten är ett enskilt tecken. false anger att den grundläggande enheten är ett helt ord.

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


Anger om dra och släpp är aktiverat för kontrollen.

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


Anger om användaren kan skriva i kontrollen.

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


Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Anger om data i kontrollen är låst för redigering.

**Returns:**
boolean
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


Anger om kontrollen kan visa mer än en rad text.

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


Anger om kontrollen är transparent.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Anger om den här kontrollen är synlig.

**Returns:**
boolean
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad.

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


Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


Anger om fokus automatiskt kommer att flyttas till nästa kontroll när användaren anger det maximala antalet tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Anger den grundläggande enheten som används för att utöka ett urval. True anger att den grundläggande enheten är ett enskilt tecken. false anger att den grundläggande enheten är ett helt ord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Ställer in OLE-färgen för bakgrunden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Ställer in OLE-färgen för bakgrunden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Ställer in typen av ram som används av kontrollen.

Se [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Anger om dra och släpp är aktiverat för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Anger symbolen som visas på rullknappen

Se [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Anger om användaren kan skriva i kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Anger urvalsbeteende när kontrollen öppnas. True anger att urvalet förblir oförändrat från senaste gången kontrollen var aktiv. False anger att all text i kontrollen kommer att markeras när kontrollen öppnas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


Anger beteendet för ENTER-tangenten. True betyder att tryck på ENTER skapar en ny rad. False betyder att tryck på ENTER flyttar fokus till nästa objekt i tabb-ordningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Ställer in OLE-färgen för förgrunden.

**Remarks**

Gäller inte för bildkontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Ställer in höjden på kontrollen i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Ställer in standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus.

Se [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


Indikerar om kontrollen endast visar kompletta textrader utan att visa några partiella rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Ställer in den länkade cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Ställer in listfyllningsområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Anger om data i kontrollen är låst för redigering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Ställer in maximalt antal tecken

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Ställer in en anpassad ikon som ska visas som muspekare för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Ställer in typen av ikon som visas som muspekare för kontrollen.

Se [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


Anger om kontrollen kan visa mer än en rad text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


Ställer in ett tecken som ska visas i stället för de inmatade tecknen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Indikerar om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen.

Se [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indikerar om en skugga ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Anger symbolen som visas på rullknappen

Se [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Ställer in den speciella effekten för kontrollen.

Se [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


Indikerar om tabulatortecken är tillåtna i kontrollens text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ställer in texten för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Representerar hur texten som används av kontrollen ska justeras.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Anger om kontrollen är transparent.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Anger om den här kontrollen är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Ställer in bredden på kontrollen i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

