---
title: "ComboBoxActiveXControl"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein ComboBox-ActiveX-Steuerelement dar."
type: docs
url: /de/java/com.aspose.cells/comboboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ComboBoxActiveXControl extends ActiveXControl
```

Stellt ein ComboBox-ActiveX-Steuerelement dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Liefert die OLE-Farbe des Hintergrunds. |
| [getBorderOleColor()](#getBorderOleColor--) | Liefert die OLE-Farbe des Hintergrunds. |
| [getBorderStyle()](#getBorderStyle--) | Liefert den von der Steuerung verwendeten Rahmentyp. |
| [getBoundColumn()](#getBoundColumn--) | Gibt an, wie die Value-Eigenschaft für ein ComboBox- oder ListBox-Steuerelement bestimmt wird, wenn der Wert der MultiSelect-Eigenschaft (fmMultiSelectSingle) ist. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Gibt die Anzahl der Spalten an, die in einem ComboBox- oder ListBox-Steuerelement angezeigt werden. |
| [getColumnWidths()](#getColumnWidths--) | Ermittelt die Breite der Spalte. |
| [getData()](#getData--) | Ermittelt die Binärdaten des Steuerelements. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Gibt das Auswahlverhalten beim Betreten des Steuerelements an. |
| [getFont()](#getFont--) | Stellt die Schriftart des Steuerelements dar. |
| [getForeOleColor()](#getForeOleColor--) | Ermittelt die OLE-Farbe des Vordergrunds. |
| [getHeight()](#getHeight--) | Ermittelt die Höhe des Steuerelements in Punkten. |
| [getHideSelection()](#getHideSelection--) | Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat. |
| [getIMEMode()](#getIMEMode--) | Ermittelt den Standardlaufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält. |
| [getLinkedCell()](#getLinkedCell--) | Ermittelt die verknüpfte Zelle. |
| [getListFillRange()](#getListFillRange--) | Ermittelt den Ausfüllbereich der Liste. |
| [getListRows()](#getListRows--) | Stellt die maximale Anzahl von Zeilen dar, die in der Liste angezeigt werden. |
| [getListStyle()](#getListStyle--) | Ermittelt das visuelle Erscheinungsbild. |
| [getListWidth()](#getListWidth--) | Ermittelt die Breite in Punkten. |
| [getMatchEntry()](#getMatchEntry--) | Gibt an, wie eine ListBox oder ComboBox ihre Liste durchsucht, während der Benutzer tippt. |
| [getMaxLength()](#getMaxLength--) | Ermittelt die maximale Anzahl von Zeichen |
| [getMouseIcon()](#getMouseIcon--) | Ermittelt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getMousePointer()](#getMousePointer--) | Ermittelt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getSelectionMargin()](#getSelectionMargin--) | Gibt an, ob der Benutzer eine Textzeile auswählen kann, indem er in den Bereich links vom Text klickt. |
| [getShadow()](#getShadow--) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Gibt an, ob Spaltenüberschriften angezeigt werden. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird |
| [getSpecialEffect()](#getSpecialEffect--) | Ermittelt den Spezialeffekt des Steuerelements. |
| [getTextAlign()](#getTextAlign--) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [getTextColumn()](#getTextColumn--) | Stellt die Spalte in einer ComboBox oder ListBox dar, die dem Benutzer angezeigt wird. |
| [getType()](#getType--) | Ermittelt den Typ des ActiveX-Steuerelements. |
| [getValue()](#getValue--) | Liest den Wert des Steuerelements. |
| [getWidth()](#getWidth--) | Liest die Breite des Steuerelements in Punkten. |
| [getWorkbook()](#getWorkbook--) | Liest das [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) Objekt. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist. |
| [isEditable()](#isEditable--) | Gibt an, ob der Benutzer in das Steuerelement tippen kann. |
| [isEnabled()](#isEnabled--) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [isLocked()](#isLocked--) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [isTransparent()](#isTransparent--) | Gibt an, ob das Steuerelement transparent ist. |
| [isVisible()](#isVisible--) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Legt die OLE-Farbe des Hintergrunds fest. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Legt die OLE-Farbe des Hintergrunds fest. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Legt den vom Steuerelement verwendeten Rahmentyp fest. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Gibt an, wie die Value-Eigenschaft für ein ComboBox- oder ListBox-Steuerelement bestimmt wird, wenn der Wert der MultiSelect-Eigenschaft (fmMultiSelectSingle) ist. |
| [setColumnCount(int value)](#setColumnCount-int-) | Gibt die Anzahl der Spalten an, die in einem ComboBox- oder ListBox-Steuerelement angezeigt werden. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Legt die Breite der Spalte fest. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird |
| [setEditable(boolean value)](#setEditable-boolean-) | Gibt an, ob der Benutzer in das Steuerelement tippen kann. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Gibt das Auswahlverhalten beim Betreten des Steuerelements an. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Legt die OLE-Farbe des Vordergrunds fest. |
| [setHeight(double value)](#setHeight-double-) | Legt die Höhe des Steuerelements in Punkten fest. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat. |
| [setIMEMode(int value)](#setIMEMode-int-) | Legt den Standard‑Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement fest, wenn es den Fokus erhält. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Legt die verknüpfte Zelle fest. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Legt den Listenfüllbereich fest. |
| [setListRows(int value)](#setListRows-int-) | Stellt die maximale Anzahl von Zeilen dar, die in der Liste angezeigt werden. |
| [setListStyle(int value)](#setListStyle-int-) | Legt das visuelle Erscheinungsbild fest. |
| [setListWidth(double value)](#setListWidth-double-) | Legt die Breite in Punkten fest. |
| [setLocked(boolean value)](#setLocked-boolean-) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Gibt an, wie eine ListBox oder ComboBox ihre Liste durchsucht, während der Benutzer tippt. |
| [setMaxLength(int value)](#setMaxLength-int-) | Legt die maximale Anzahl von Zeichen fest |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setMousePointer(int value)](#setMousePointer-int-) | Legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setSelectionMargin(boolean value)](#setSelectionMargin-boolean-) | Gibt an, ob der Benutzer eine Textzeile auswählen kann, indem er in den Bereich links vom Text klickt. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Gibt an, ob Spaltenüberschriften angezeigt werden. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Legt den Spezialeffekt des Steuerelements fest. |
| [setTextAlign(int value)](#setTextAlign-int-) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [setTextColumn(int value)](#setTextColumn-int-) | Stellt die Spalte in einer ComboBox oder ListBox dar, die dem Benutzer angezeigt wird. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Gibt an, ob das Steuerelement transparent ist. |
| [setValue(String value)](#setValue-java.lang.String-) | Legt den Wert des Steuerelements fest. |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [setWidth(double value)](#setWidth-double-) | Legt die Breite des Steuerelements in Punkten fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Liefert die OLE-Farbe des Hintergrunds.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Liefert die OLE-Farbe des Hintergrunds.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Liefert den von der Steuerung verwendeten Rahmentyp.

Siehe [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


Gibt an, wie die Value-Eigenschaft für ein ComboBox- oder ListBox-Steuerelement bestimmt wird, wenn der Wert der MultiSelect-Eigenschaft (fmMultiSelectSingle) ist.

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


Gibt die Anzahl der Spalten an, die in einem ComboBox- oder ListBox-Steuerelement angezeigt werden.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Ermittelt die Breite der Spalte.

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


Ermittelt die Binärdaten des Steuerelements.

**Returns:**
byte[]
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird

Siehe [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True gibt an, dass die Auswahl unverändert bleibt seit dem letzten Mal, als das Steuerelement aktiv war. False gibt an, dass beim Betreten des Steuerelements der gesamte Text im Steuerelement ausgewählt wird.

**Returns:**
boolean
### getFont() {#getFont--}
```
public Font getFont()
```


Stellt die Schriftart des Steuerelements dar.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Ermittelt die OLE-Farbe des Vordergrunds.

**Remarks**

Gilt nicht für das Image-Steuerelement.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Ermittelt die Höhe des Steuerelements in Punkten.

**Returns:**
double
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat.

**Returns:**
boolean
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Ermittelt den Standardlaufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält.

Siehe [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Ermittelt die verknüpfte Zelle.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Ermittelt den Ausfüllbereich der Liste.

**Returns:**
java.lang.String
### getListRows() {#getListRows--}
```
public int getListRows()
```


Stellt die maximale Anzahl von Zeilen dar, die in der Liste angezeigt werden.

**Returns:**
int
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Ermittelt das visuelle Erscheinungsbild.

Siehe [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Ermittelt die Breite in Punkten.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Gibt an, wie eine ListBox oder ComboBox ihre Liste durchsucht, während der Benutzer tippt.

Siehe [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Returns:**
int
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Ermittelt die maximale Anzahl von Zeichen

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Ermittelt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Ermittelt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird.

Siehe [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getSelectionMargin() {#getSelectionMargin--}
```
public boolean getSelectionMargin()
```


Gibt an, ob der Benutzer eine Textzeile auswählen kann, indem er in den Bereich links vom Text klickt.

**Returns:**
boolean
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Gibt an, ob ein Schatten angezeigt werden soll.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Gibt an, ob Spaltenüberschriften angezeigt werden.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird

Siehe [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Ermittelt den Spezialeffekt des Steuerelements.

Siehe [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Stellt die Spalte in einer ComboBox oder ListBox dar, die dem Benutzer angezeigt wird.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Ermittelt den Typ des ActiveX-Steuerelements.

Siehe [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


Liest den Wert des Steuerelements.

**Returns:**
java.lang.String
### getWidth() {#getWidth--}
```
public double getWidth()
```


Liest die Breite des Steuerelements in Punkten.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Liest das [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) Objekt.

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


Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen.

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist.

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist.

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Gibt an, ob der Benutzer in das Steuerelement tippen kann.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Gibt an, ob das Steuerelement transparent ist.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Gibt an, ob dieses Steuerelement sichtbar ist.

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


Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Legt die OLE-Farbe des Hintergrunds fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Legt die OLE-Farbe des Hintergrunds fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Legt den vom Steuerelement verwendeten Rahmentyp fest.

Siehe [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


Gibt an, wie die Value-Eigenschaft für ein ComboBox- oder ListBox-Steuerelement bestimmt wird, wenn der Wert der MultiSelect-Eigenschaft (fmMultiSelectSingle) ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


Gibt die Anzahl der Spalten an, die in einem ComboBox- oder ListBox-Steuerelement angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Legt die Breite der Spalte fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird

Siehe [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Gibt an, ob der Benutzer in das Steuerelement tippen kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True gibt an, dass die Auswahl unverändert bleibt seit dem letzten Mal, als das Steuerelement aktiv war. False gibt an, dass beim Betreten des Steuerelements der gesamte Text im Steuerelement ausgewählt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Legt die OLE-Farbe des Vordergrunds fest.

**Remarks**

Gilt nicht für das Image-Steuerelement.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Legt die Höhe des Steuerelements in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Legt den Standard‑Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement fest, wenn es den Fokus erhält.

Siehe [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Legt die verknüpfte Zelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Legt den Listenfüllbereich fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setListRows(int value) {#setListRows-int-}
```
public void setListRows(int value)
```


Stellt die maximale Anzahl von Zeilen dar, die in der Liste angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Legt das visuelle Erscheinungsbild fest.

Siehe [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Legt die Breite in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Gibt an, wie eine ListBox oder ComboBox ihre Liste durchsucht, während der Benutzer tippt.

Siehe [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Legt die maximale Anzahl von Zeichen fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird.

Siehe [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSelectionMargin(boolean value) {#setSelectionMargin-boolean-}
```
public void setSelectionMargin(boolean value)
```


Gibt an, ob der Benutzer eine Textzeile auswählen kann, indem er in den Bereich links vom Text klickt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Gibt an, ob ein Schatten angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Gibt an, ob Spaltenüberschriften angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird

Siehe [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Legt den Spezialeffekt des Steuerelements fest.

Siehe [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Stellt die Spalte in einer ComboBox oder ListBox dar, die dem Benutzer angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Gibt an, ob das Steuerelement transparent ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Legt den Wert des Steuerelements fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Gibt an, ob dieses Steuerelement sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Legt die Breite des Steuerelements in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

