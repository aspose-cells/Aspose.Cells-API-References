---
title: "ScrollBarActiveXControl"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die ScrollBar-Steuerung dar."
type: docs
url: /de/java/com.aspose.cells/scrollbaractivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol), [com.aspose.cells.SpinButtonActiveXControl](../../com.aspose.cells/spinbuttonactivexcontrol)
```
public class ScrollBarActiveXControl extends SpinButtonActiveXControl
```

Stellt die ScrollBar-Steuerung dar.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a ToggleButtonActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.SCROLL_BAR, 1, 0, 1, 0, 100, 50);
         ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Liefert die OLE-Farbe des Hintergrunds. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Ermittelt die Binärdaten des Steuerelements. |
| [getFont()](#getFont--) | Stellt die Schriftart des Steuerelements dar. |
| [getForeOleColor()](#getForeOleColor--) | Ermittelt die OLE-Farbe des Vordergrunds. |
| [getHeight()](#getHeight--) | Ermittelt die Höhe des Steuerelements in Punkten. |
| [getIMEMode()](#getIMEMode--) | Ermittelt den Standardlaufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält. |
| [getLargeChange()](#getLargeChange--) | Ermittelt den Betrag, um den sich die Position-Eigenschaft ändert. |
| [getLinkedCell()](#getLinkedCell--) | Ermittelt die verknüpfte Zelle. |
| [getListFillRange()](#getListFillRange--) | Ermittelt den Ausfüllbereich der Liste. |
| [getMax()](#getMax--) | Ermittelt den maximal zulässigen Wert. |
| [getMin()](#getMin--) | Ermittelt den minimal zulässigen Wert. |
| [getMouseIcon()](#getMouseIcon--) | Ermittelt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getMousePointer()](#getMousePointer--) | Ermittelt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getOrientation()](#getOrientation--) | Ermittelt, ob die SpinButton- oder ScrollBar-Steuerung vertikal oder horizontal ausgerichtet ist. |
| [getPosition()](#getPosition--) | Ermittelt den Wert. |
| [getShadow()](#getShadow--) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [getSmallChange()](#getSmallChange--) | Ermittelt den Betrag, um den sich die Position-Eigenschaft ändert. |
| [getTextAlign()](#getTextAlign--) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [getType()](#getType--) | Ermittelt den Typ des ActiveX-Steuerelements. |
| [getWidth()](#getWidth--) | Liest die Breite des Steuerelements in Punkten. |
| [getWorkbook()](#getWorkbook--) | Liest das [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) Objekt. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [isEnabled()](#isEnabled--) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [isLocked()](#isLocked--) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [isTransparent()](#isTransparent--) | Gibt an, ob das Steuerelement transparent ist. |
| [isVisible()](#isVisible--) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Legt die OLE-Farbe des Hintergrunds fest. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Legt die OLE-Farbe des Vordergrunds fest. |
| [setHeight(double value)](#setHeight-double-) | Legt die Höhe des Steuerelements in Punkten fest. |
| [setIMEMode(int value)](#setIMEMode-int-) | Legt den Standard‑Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement fest, wenn es den Fokus erhält. |
| [setLargeChange(int value)](#setLargeChange-int-) | Legt den Betrag fest, um den sich die Position-Eigenschaft ändert. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Legt die verknüpfte Zelle fest. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Legt den Listenfüllbereich fest. |
| [setLocked(boolean value)](#setLocked-boolean-) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [setMax(int value)](#setMax-int-) | Legt den maximal zulässigen Wert fest. |
| [setMin(int value)](#setMin-int-) | Legt den minimal zulässigen Wert fest. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setMousePointer(int value)](#setMousePointer-int-) | Legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setOrientation(int value)](#setOrientation-int-) | Legt fest, ob die SpinButton- oder ScrollBar-Steuerung vertikal oder horizontal ausgerichtet ist. |
| [setPosition(int value)](#setPosition-int-) | Legt den Wert fest. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [setSmallChange(int value)](#setSmallChange-int-) | Legt den Betrag fest, um den sich die Position-Eigenschaft ändert. |
| [setTextAlign(int value)](#setTextAlign-int-) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Gibt an, ob das Steuerelement transparent ist. |
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


Ermittelt die Binärdaten des Steuerelements.

**Returns:**
byte[]
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
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Ermittelt den Standardlaufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält.

Siehe [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getLargeChange() {#getLargeChange--}
```
public int getLargeChange()
```


Ermittelt den Betrag, um den sich die Position-Eigenschaft ändert.

**Example**

```
         activeXControl.setLargeChange(5);
```

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
### getMax() {#getMax--}
```
public int getMax()
```


Ermittelt den maximal zulässigen Wert.

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


Ermittelt den minimal zulässigen Wert.

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
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Ermittelt, ob die SpinButton- oder ScrollBar-Steuerung vertikal oder horizontal ausgerichtet ist.

Siehe [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).

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


Ermittelt den Wert.

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


Gibt an, ob ein Schatten angezeigt werden soll.

**Returns:**
boolean
### getSmallChange() {#getSmallChange--}
```
public int getSmallChange()
```


Ermittelt den Betrag, um den sich die Position-Eigenschaft ändert.

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


Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Ermittelt den Typ des ActiveX-Steuerelements.

Siehe [ControlType](../../com.aspose.cells/controltype).

**Example**

```
         if(activeXControl.getType() == com.aspose.cells.ControlType.SCROLL_BAR)
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

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Legt die OLE-Farbe des Hintergrunds fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann.

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

### setLargeChange(int value) {#setLargeChange-int-}
```
public void setLargeChange(int value)
```


Legt den Betrag fest, um den sich die Position-Eigenschaft ändert.

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMax(int value) {#setMax-int-}
```
public void setMax(int value)
```


Legt den maximal zulässigen Wert fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMin(int value) {#setMin-int-}
```
public void setMin(int value)
```


Legt den minimal zulässigen Wert fest.

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

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Legt fest, ob die SpinButton- oder ScrollBar-Steuerung vertikal oder horizontal ausgerichtet ist.

Siehe [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Legt den Wert fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Gibt an, ob ein Schatten angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSmallChange(int value) {#setSmallChange-int-}
```
public void setSmallChange(int value)
```


Legt den Betrag fest, um den sich die Position-Eigenschaft ändert.

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Gibt an, ob das Steuerelement transparent ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

