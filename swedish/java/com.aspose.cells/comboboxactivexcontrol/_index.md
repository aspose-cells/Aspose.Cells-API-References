---
title: "ComboBoxActiveXControl"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en ComboBox ActiveX-kontroll."
type: docs
url: /sv/java/com.aspose.cells/comboboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ComboBoxActiveXControl extends ActiveXControl
```

Representerar en ComboBox ActiveX-kontroll.
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
| [getDropButtonStyle()](#getDropButtonStyle--) | Anger symbolen som visas på rullknappen |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Anger markeringsbeteende när kontrollen aktiveras. |
| [getFont()](#getFont--) | Representerar kontrollens teckensnitt. |
| [getForeOleColor()](#getForeOleColor--) | Hämtar förgrundens OLE-färg. |
| [getHeight()](#getHeight--) | Hämtar kontrollens höjd i punktenheter. |
| [getHideSelection()](#getHideSelection--) | Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus. |
| [getIMEMode()](#getIMEMode--) | Hämtar standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [getLinkedCell()](#getLinkedCell--) | Hämtar den länkade cellen. |
| [getListFillRange()](#getListFillRange--) | Hämtar listans fyllningsintervall. |
| [getListRows()](#getListRows--) | Representerar det maximala antalet rader som ska visas i listan. |
| [getListStyle()](#getListStyle--) | Hämtar det visuella utseendet. |
| [getListWidth()](#getListWidth--) | Hämtar bredden i punktenheter. |
| [getMatchEntry()](#getMatchEntry--) | Indikerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver. |
| [getMaxLength()](#getMaxLength--) | Hämtar det maximala antalet tecken |
| [getMouseIcon()](#getMouseIcon--) | Hämtar en anpassad ikon som ska visas som muspekare för kontrollen. |
| [getMousePointer()](#getMousePointer--) | Hämtar typen av ikon som visas som muspekare för kontrollen. |
| [getSelectionMargin()](#getSelectionMargin--) | Indikerar om användaren kan markera en textrad genom att klicka i området till vänster om texten. |
| [getShadow()](#getShadow--) | Indikerar om en skugga ska visas. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Indikerar om kolumnrubriker visas. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Anger symbolen som visas på rullknappen |
| [getSpecialEffect()](#getSpecialEffect--) | Hämtar kontrollens specialeffekt. |
| [getTextAlign()](#getTextAlign--) | Representerar hur texten som används av kontrollen ska justeras. |
| [getTextColumn()](#getTextColumn--) | Representerar kolumnen i en ComboBox eller ListBox som ska visas för användaren. |
| [getType()](#getType--) | Hämtar typen av ActiveX-kontrollen. |
| [getValue()](#getValue--) | Hämtar värdet för kontrollen. |
| [getWidth()](#getWidth--) | Hämtar bredden på kontrollen i enheten punkter. |
| [getWorkbook()](#getWorkbook--) | Hämtar [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) objektet. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Anger den grundläggande enheten som används för att utöka en markering. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Anger om dra och släpp är aktiverat för kontrollen. |
| [isEditable()](#isEditable--) | Anger om användaren kan skriva i kontrollen. |
| [isEnabled()](#isEnabled--) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [isLocked()](#isLocked--) | Anger om data i kontrollen är låst för redigering. |
| [isTransparent()](#isTransparent--) | Anger om kontrollen är transparent. |
| [isVisible()](#isVisible--) | Anger om den här kontrollen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Anger den grundläggande enheten som används för att utöka en markering. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Ställer in OLE-färgen för bakgrunden. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Ställer in typen av ram som används av kontrollen. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Representerar hur Value-egenskapen bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | Representerar antalet kolumner som ska visas i en ComboBox eller ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Ställer in bredden på kolumnen. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Anger om dra och släpp är aktiverat för kontrollen. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Anger symbolen som visas på rullknappen |
| [setEditable(boolean value)](#setEditable-boolean-) | Anger om användaren kan skriva i kontrollen. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Anger markeringsbeteende när kontrollen aktiveras. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Ställer in OLE-färgen för förgrunden. |
| [setHeight(double value)](#setHeight-double-) | Ställer in höjden på kontrollen i enheten punkter. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus. |
| [setIMEMode(int value)](#setIMEMode-int-) | Ställer in standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Ställer in den länkade cellen. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Ställer in listfyllningsområdet. |
| [setListRows(int value)](#setListRows-int-) | Representerar det maximala antalet rader som ska visas i listan. |
| [setListStyle(int value)](#setListStyle-int-) | Ställer in det visuella utseendet. |
| [setListWidth(double value)](#setListWidth-double-) | Ställer in bredden i enheten punkter. |
| [setLocked(boolean value)](#setLocked-boolean-) | Anger om data i kontrollen är låst för redigering. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Indikerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver. |
| [setMaxLength(int value)](#setMaxLength-int-) | Ställer in maximalt antal tecken |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Ställer in en anpassad ikon som ska visas som muspekare för kontrollen. |
| [setMousePointer(int value)](#setMousePointer-int-) | Ställer in typen av ikon som visas som muspekare för kontrollen. |
| [setSelectionMargin(boolean value)](#setSelectionMargin-boolean-) | Indikerar om användaren kan markera en textrad genom att klicka i området till vänster om texten. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indikerar om en skugga ska visas. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Indikerar om kolumnrubriker visas. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Anger symbolen som visas på rullknappen |
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
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Anger symbolen som visas på rullknappen

Se [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Anger urvalsbeteende när kontrollen öppnas. True anger att urvalet förblir oförändrat från senaste gången kontrollen var aktiv. False anger att all text i kontrollen kommer att markeras när kontrollen öppnas.

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
### getListRows() {#getListRows--}
```
public int getListRows()
```


Representerar det maximala antalet rader som ska visas i listan.

**Returns:**
int
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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Hämtar det maximala antalet tecken

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
### getSelectionMargin() {#getSelectionMargin--}
```
public boolean getSelectionMargin()
```


Indikerar om användaren kan markera en textrad genom att klicka i området till vänster om texten.

**Returns:**
boolean
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
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Anger symbolen som visas på rullknappen

Se [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Returns:**
int
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
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Anger den grundläggande enheten som används för att utöka ett urval. True anger att den grundläggande enheten är ett enskilt tecken. false anger att den grundläggande enheten är ett helt ord.

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Anger om dra och släpp är aktiverat för kontrollen.

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Anger om användaren kan skriva i kontrollen.

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

### setListRows(int value) {#setListRows-int-}
```
public void setListRows(int value)
```


Representerar det maximala antalet rader som ska visas i listan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setSelectionMargin(boolean value) {#setSelectionMargin-boolean-}
```
public void setSelectionMargin(boolean value)
```


Indikerar om användaren kan markera en textrad genom att klicka i området till vänster om texten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

