---
title: "ListBoxActiveXControl"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en ListBox ActiveX-kontroll."
type: docs
url: /sv/java/com.aspose.cells/listboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ListBoxActiveXControl extends ActiveXControl
```

Representerar en ListBox ActiveX-kontroll.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Hämtar ole-färgen för bakgrunden. |
| [getBorderOleColor()](#getBorderOleColor--) | Hämtar ole-färgen för bakgrunden. |
| [getBorderStyle()](#getBorderStyle--) | Hämtar typen av kant som används av kontrollen. |
| [getBoundColumn()](#getBoundColumn--) | Representerar hur Value-egenskapen bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Representerar antalet kolumner som ska visas i en ComboBox eller ListBox. |
| [getColumnWidths()](#getColumnWidths--) | Hämtar kolumnens bredd. |
| [getData()](#getData--) | Hämtar kontrollens binära data. |
| [getFont()](#getFont--) | Representerar kontrollens teckensnitt. |
| [getForeOleColor()](#getForeOleColor--) | Hämtar förgrundens OLE-färg. |
| [getHeight()](#getHeight--) | Hämtar kontrollens höjd i punktenheter. |
| [getIMEMode()](#getIMEMode--) | Hämtar standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [getIntegralHeight()](#getIntegralHeight--) | Indikerar om kontrollen endast visar kompletta textrader utan att visa några partiella rader. |
| [getLinkedCell()](#getLinkedCell--) | Hämtar den länkade cellen. |
| [getListFillRange()](#getListFillRange--) | Hämtar listans fyllningsintervall. |
| [getListStyle()](#getListStyle--) | Hämtar det visuella utseendet. |
| [getListWidth()](#getListWidth--) | Hämtar bredden i punktenheter. |
| [getMatchEntry()](#getMatchEntry--) | Indikerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver. |
| [getMouseIcon()](#getMouseIcon--) | Hämtar en anpassad ikon som ska visas som muspekare för kontrollen. |
| [getMousePointer()](#getMousePointer--) | Hämtar typen av ikon som visas som muspekare för kontrollen. |
| [getScrollBars()](#getScrollBars--) | Indikerar om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen. |
| [getSelectionType()](#getSelectionType--) | Indikerar om kontrollen tillåter flera val. |
| [getShadow()](#getShadow--) | Indikerar om en skugga ska visas. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Indikerar om kolumnrubriker visas. |
| [getSpecialEffect()](#getSpecialEffect--) | Hämtar kontrollens specialeffekt. |
| [getTextAlign()](#getTextAlign--) | Representerar hur texten som används av kontrollen ska justeras. |
| [getTextColumn()](#getTextColumn--) | Representerar kolumnen i en ComboBox eller ListBox som ska visas för användaren. |
| [getType()](#getType--) | Hämtar typen av ActiveX-kontrollen. |
| [getValue()](#getValue--) | Hämtar värdet för kontrollen. |
| [getWidth()](#getWidth--) | Hämtar bredden på kontrollen i enheten punkter. |
| [getWorkbook()](#getWorkbook--) | Hämtar [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) objektet. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [isEnabled()](#isEnabled--) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [isLocked()](#isLocked--) | Anger om data i kontrollen är låst för redigering. |
| [isTransparent()](#isTransparent--) | Anger om kontrollen är transparent. |
| [isVisible()](#isVisible--) | Anger om den här kontrollen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Ställer in typen av ram som används av kontrollen. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Representerar hur Value-egenskapen bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | Representerar antalet kolumner som ska visas i en ComboBox eller ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Ställer in bredden på kolumnen. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ställer in OLE-färgen för förgrunden. |
| [setHeight(double value)](#setHeight-double-) | Ställer in höjden på kontrollen i enheten punkter. |
| [setIMEMode(int value)](#setIMEMode-int-) | Ställer in standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indikerar om kontrollen endast visar kompletta textrader utan att visa några partiella rader. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Ställer in den länkade cellen. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Ställer in listfyllningsområdet. |
| [setListStyle(int value)](#setListStyle-int-) | Ställer in det visuella utseendet. |
| [setListWidth(double value)](#setListWidth-double-) | Ställer in bredden i enheten punkter. |
| [setLocked(boolean value)](#setLocked-boolean-) | Anger om data i kontrollen är låst för redigering. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Indikerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Ställer in en anpassad ikon som ska visas som muspekare för kontrollen. |
| [setMousePointer(int value)](#setMousePointer-int-) | Ställer in typen av ikon som visas som muspekare för kontrollen. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indikerar om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen. |
| [setSelectionType(int value)](#setSelectionType-int-) | Indikerar om kontrollen tillåter flera val. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indikerar om en skugga ska visas. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Indikerar om kolumnrubriker visas. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Ställer in den speciella effekten för kontrollen. |
| [setTextAlign(int value)](#setTextAlign-int-) | Representerar hur texten som används av kontrollen ska justeras. |
| [setTextColumn(int value)](#setTextColumn-int-) | Representerar kolumnen i en ComboBox eller ListBox som ska visas för användaren. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Anger om kontrollen är transparent. |
| [setValue(String value)](#setValue-java.lang.String-) | Ställer in värdet för kontrollen. |
| [setVisible(boolean value)](#setVisible-boolean-) | Anger om den här kontrollen är synlig. |
| [setWidth(double value)](#setWidth-double-) | Ställer in bredden på kontrollen i enheten punkter. |
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

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Hämtar typen av kant som används av kontrollen.

Se [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


Representerar hur Value-egenskapen bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är (fmMultiSelectSingle).

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


Representerar antalet kolumner som ska visas i en ComboBox eller ListBox.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Hämtar kolumnens bredd.

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


Hämtar kontrollens binära data.

**Returns:**
byte[]
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
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Hämtar det visuella utseendet.

Se [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Hämtar bredden i punktenheter.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Indikerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver.

Se [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

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
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indikerar om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen.

Se [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Returns:**
int
### getSelectionType() {#getSelectionType--}
```
public int getSelectionType()
```


Indikerar om kontrollen tillåter flera val.

Se [SelectionType](../../com.aspose.cells/selectiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indikerar om en skugga ska visas.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Indikerar om kolumnrubriker visas.

**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Hämtar kontrollens specialeffekt.

Se [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Representerar hur texten som används av kontrollen ska justeras.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Representerar kolumnen i en ComboBox eller ListBox som ska visas för användaren.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av ActiveX-kontrollen.

Se [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


Hämtar värdet för kontrollen.

**Remarks**

Gäller endast när [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) är SelectionType.Single;

**Returns:**
java.lang.String
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

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


Representerar hur Value-egenskapen bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är (fmMultiSelectSingle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


Representerar antalet kolumner som ska visas i en ComboBox eller ListBox.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Ställer in bredden på kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser.

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

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Ställer in det visuella utseendet.

Se [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Ställer in bredden i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Anger om data i kontrollen är låst för redigering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Indikerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver.

Se [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

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

### setSelectionType(int value) {#setSelectionType-int-}
```
public void setSelectionType(int value)
```


Indikerar om kontrollen tillåter flera val.

Se [SelectionType](../../com.aspose.cells/selectiontype).

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

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Indikerar om kolumnrubriker visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Representerar kolumnen i en ComboBox eller ListBox som ska visas för användaren.

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

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Ställer in värdet för kontrollen.

**Remarks**

Gäller endast när [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) är SelectionType.Single;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

