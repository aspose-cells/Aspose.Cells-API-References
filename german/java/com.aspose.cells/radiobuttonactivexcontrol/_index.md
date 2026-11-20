---
title: "RadioButtonActiveXControl"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein RadioButton‑ActiveX‑Steuerelement dar."
type: docs
url: /de/java/com.aspose.cells/radiobuttonactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol), [com.aspose.cells.ToggleButtonActiveXControl](../../com.aspose.cells/togglebuttonactivexcontrol)
```
public class RadioButtonActiveXControl extends ToggleButtonActiveXControl
```

Stellt ein RadioButton‑ActiveX‑Steuerelement dar.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a ToggleButtonActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.RADIO_BUTTON, 1, 0, 1, 0, 100, 50);
         RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccelerator()](#getAccelerator--) | Ruft die Beschleunigungstaste für das Steuerelement ab. |
| [getAlignment()](#getAlignment--) | Ruft die Position der Beschriftung relativ zum Steuerelement ab. |
| [getBackOleColor()](#getBackOleColor--) | Liefert die OLE-Farbe des Hintergrunds. |
| [getCaption()](#getCaption--) | Ruft den beschreibenden Text ab, der auf einem Steuerelement angezeigt wird. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Ermittelt die Binärdaten des Steuerelements. |
| [getFont()](#getFont--) | Stellt die Schriftart des Steuerelements dar. |
| [getForeOleColor()](#getForeOleColor--) | Ermittelt die OLE-Farbe des Vordergrunds. |
| [getGroupName()](#getGroupName--) | Ruft den Namen der Gruppe ab. |
| [getHeight()](#getHeight--) | Ermittelt die Höhe des Steuerelements in Punkten. |
| [getIMEMode()](#getIMEMode--) | Ermittelt den Standardlaufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält. |
| [getLinkedCell()](#getLinkedCell--) | Ermittelt die verknüpfte Zelle. |
| [getListFillRange()](#getListFillRange--) | Ermittelt den Ausfüllbereich der Liste. |
| [getMouseIcon()](#getMouseIcon--) | Ermittelt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getMousePointer()](#getMousePointer--) | Ermittelt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getPicture()](#getPicture--) | Ruft die Daten des Bildes ab. |
| [getPicturePosition()](#getPicturePosition--) | Ruft den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung ab. |
| [getShadow()](#getShadow--) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [getSpecialEffect()](#getSpecialEffect--) | Ermittelt den Spezialeffekt des Steuerelements. |
| [getTextAlign()](#getTextAlign--) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [getType()](#getType--) | Ermittelt den Typ des ActiveX-Steuerelements. |
| [getValue()](#getValue--) | Gibt an, ob das Steuerelement aktiviert ist oder nicht. |
| [getWidth()](#getWidth--) | Liest die Breite des Steuerelements in Punkten. |
| [getWorkbook()](#getWorkbook--) | Liest das [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) Objekt. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [isEnabled()](#isEnabled--) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [isLocked()](#isLocked--) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [isTransparent()](#isTransparent--) | Gibt an, ob das Steuerelement transparent ist. |
| [isTripleState()](#isTripleState--) | Gibt an, wie das angegebene Steuerelement Nullwerte anzeigen wird. |
| [isVisible()](#isVisible--) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [isWordWrapped()](#isWordWrapped--) | Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccelerator(char value)](#setAccelerator-char-) | Setzt die Beschleunigungstaste für das Steuerelement. |
| [setAlignment(int value)](#setAlignment-int-) | Setzt die Position der Beschriftung relativ zum Steuerelement. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Legt die OLE-Farbe des Hintergrunds fest. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Setzt den beschreibenden Text, der auf einem Steuerelement angezeigt wird. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Legt die OLE-Farbe des Vordergrunds fest. |
| [setGroupName(String value)](#setGroupName-java.lang.String-) | Setzt den Namen der Gruppe. |
| [setHeight(double value)](#setHeight-double-) | Legt die Höhe des Steuerelements in Punkten fest. |
| [setIMEMode(int value)](#setIMEMode-int-) | Legt den Standard‑Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement fest, wenn es den Fokus erhält. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Legt die verknüpfte Zelle fest. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Legt den Listenfüllbereich fest. |
| [setLocked(boolean value)](#setLocked-boolean-) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setMousePointer(int value)](#setMousePointer-int-) | Legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setPicture(byte[] value)](#setPicture-byte---) | Setzt die Daten des Bildes. |
| [setPicturePosition(int value)](#setPicturePosition-int-) | Setzt den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Legt den Spezialeffekt des Steuerelements fest. |
| [setTextAlign(int value)](#setTextAlign-int-) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Gibt an, ob das Steuerelement transparent ist. |
| [setTripleState(boolean value)](#setTripleState-boolean-) | Gibt an, wie das angegebene Steuerelement Nullwerte anzeigen wird. |
| [setValue(int value)](#setValue-int-) | Gibt an, ob das Steuerelement aktiviert ist oder nicht. |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [setWidth(double value)](#setWidth-double-) | Legt die Breite des Steuerelements in Punkten fest. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird. |
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
### getAccelerator() {#getAccelerator--}
```
public char getAccelerator()
```


Ruft die Beschleunigungstaste für das Steuerelement ab.

**Example**

```
         if (' ' != activeXControl.getAccelerator())
         {
             activeXControl.setAccelerator(' ');
         }
```

**Returns:**
char
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Ruft die Position der Beschriftung relativ zum Steuerelement ab.

Siehe [ControlCaptionAlignmentType](../../com.aspose.cells/controlcaptionalignmenttype).

**Example**

```
         activeXControl.setAlignment(com.aspose.cells.ControlCaptionAlignmentType.LEFT);
```

**Returns:**
int
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Liefert die OLE-Farbe des Hintergrunds.

**Returns:**
int
### getCaption() {#getCaption--}
```
public String getCaption()
```


Ruft den beschreibenden Text ab, der auf einem Steuerelement angezeigt wird.

**Example**

```
         activeXControl.setCaption("ExampleButton");
```

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
### getGroupName() {#getGroupName--}
```
public String getGroupName()
```


Ruft den Namen der Gruppe ab.

**Example**

```
         activeXControl.setGroupName("GroupName123");
```

**Returns:**
java.lang.String
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
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


Ruft die Daten des Bildes ab.

**Example**

```
         //e.g byte[] data = File.ReadAllBytes("image.png");
         byte[] data = null;
         if(activeXControl.getPicture() != null)
         {
             activeXControl.setPicture(data);
         }
```

**Returns:**
byte[]
### getPicturePosition() {#getPicturePosition--}
```
public int getPicturePosition()
```


Ruft den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung ab.

Siehe [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

**Example**

```
         activeXControl.setPicturePosition(com.aspose.cells.ControlPicturePositionType.ABOVE_LEFT);
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
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Ermittelt den Spezialeffekt des Steuerelements.

Siehe [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
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
         if(activeXControl.getType() == com.aspose.cells.ControlType.RADIO_BUTTON)
         {
             //do something
         }
```

**Returns:**
int
### getValue() {#getValue--}
```
public int getValue()
```


Gibt an, ob das Steuerelement aktiviert ist oder nicht.

Siehe [CheckValueType](../../com.aspose.cells/checkvaluetype).

**Example**

```
         if(activeXControl.getValue() == CheckValueType.UN_CHECKED)
         {
             activeXControl.setValue(CheckValueType.CHECKED);
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
### isTripleState() {#isTripleState--}
```
public boolean isTripleState()
```


Gibt an, wie das angegebene Steuerelement Nullwerte anzeigen wird.

**Remarks**

| Einstellung | Beschreibung |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Wahr | Das Steuerelement durchläuft die Zustände für Ja-, Nein- und Nullwerte. Das Steuerelement erscheint abgedunkelt (grau), wenn seine Value‑Eigenschaft auf Null gesetzt ist. |
| Falsch | (Standard) Das Steuerelement durchläuft die Zustände für Ja- und Neinwerte. Nullwerte werden angezeigt, als wären sie Neinwerte. |

**Example**

```
         activeXControl.setTripleState(false);
```

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Gibt an, ob dieses Steuerelement sichtbar ist.

**Returns:**
boolean
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird.

**Example**

```
         if(activeXControl.isWordWrapped() == false)
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




### setAccelerator(char value) {#setAccelerator-char-}
```
public void setAccelerator(char value)
```


Setzt die Beschleunigungstaste für das Steuerelement.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Setzt die Position der Beschriftung relativ zum Steuerelement.

Siehe [ControlCaptionAlignmentType](../../com.aspose.cells/controlcaptionalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Setzt den beschreibenden Text, der auf einem Steuerelement angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

### setGroupName(String value) {#setGroupName-java.lang.String-}
```
public void setGroupName(String value)
```


Setzt den Namen der Gruppe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


Setzt die Daten des Bildes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setPicturePosition(int value) {#setPicturePosition-int-}
```
public void setPicturePosition(int value)
```


Setzt den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung.

Siehe [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Gibt an, ob das Steuerelement transparent ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTripleState(boolean value) {#setTripleState-boolean-}
```
public void setTripleState(boolean value)
```


Gibt an, wie das angegebene Steuerelement Nullwerte anzeigen wird.

**Remarks**

| Einstellung | Beschreibung |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Wahr | Das Steuerelement durchläuft die Zustände für Ja-, Nein- und Nullwerte. Das Steuerelement erscheint abgedunkelt (grau), wenn seine Value‑Eigenschaft auf Null gesetzt ist. |
| Falsch | (Standard) Das Steuerelement durchläuft die Zustände für Ja- und Neinwerte. Nullwerte werden angezeigt, als wären sie Neinwerte. |

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValue(int value) {#setValue-int-}
```
public void setValue(int value)
```


Gibt an, ob das Steuerelement aktiviert ist oder nicht.

Siehe [CheckValueType](../../com.aspose.cells/checkvaluetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

