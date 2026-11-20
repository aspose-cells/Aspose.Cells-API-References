---
title: "DefaultStyleSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Einstellungen für die Standardwerte der Stil‑Eigenschaften von Arbeitsmappen."
type: docs
url: /de/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

Einstellungen für die Standardwerte der Stil-Eigenschaften des Arbeitsbuchs.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | Gibt an, ob die Eigenschaft für das Zahlenformat vorzuziehen ist, wenn der Stil sowohl integrierte Zahlen als auch ein benutzerdefiniertes Muster definiert. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | Ermittelt den Standard‑Schriftartnamen für die Arbeitsmappe. |
| [getFontSize()](#getFontSize--) | Ermittelt die Standard‑Schriftgröße für die Arbeitsmappe. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Ermittelt den Standardwert für die horizontale Ausrichtung. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Ermittelt den Standardwert für die vertikale Ausrichtung. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | Gibt an, ob die Eigenschaft für das Zahlenformat vorzuziehen ist, wenn der Stil sowohl integrierte Zahlen als auch ein benutzerdefiniertes Muster definiert. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Legt den Standard‑Schriftartnamen für die Arbeitsmappe fest. |
| [setFontSize(double value)](#setFontSize-double-) | Legt die Standard‑Schriftgröße für die Arbeitsmappe fest. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Legt den Standardwert für die horizontale Ausrichtung fest. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Legt den Standardwert für die vertikale Ausrichtung fest |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


Gibt an, ob die Eigenschaft für das Zahlenformat vorzuziehen ist, wenn der Stil sowohl integrierte Zahl als auch benutzerdefiniertes Muster definiert. Der Standardwert ist false, das bedeutet, dass standardmäßig das benutzerdefinierte Muster verwendet wird, um Werte zu formatieren, solange es für einen Stil nicht leer ist.

**Remarks**

Beim Laden einer Arbeitsmappe aus einer vorhandenen Vorlagendatei können für einen Stil sowohl integrierte Zahl als auch benutzerdefiniertes Muster definiert sein. Diese Eigenschaft bestimmt, ob beim Formatieren von Werten mit dem Stil die integrierte Zahl oder das benutzerdefinierte Muster verwendet werden soll.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


Ermittelt den Standard‑Schriftartnamen für die Arbeitsmappe.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Ermittelt die Standard‑Schriftgröße für die Arbeitsmappe.

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Ermittelt den Standardwert für die horizontale Ausrichtung.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Ermittelt den Standardwert für die vertikale Ausrichtung.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


Gibt an, ob die Eigenschaft für das Zahlenformat vorzuziehen ist, wenn der Stil sowohl integrierte Zahl als auch benutzerdefiniertes Muster definiert. Der Standardwert ist false, das bedeutet, dass standardmäßig das benutzerdefinierte Muster verwendet wird, um Werte zu formatieren, solange es für einen Stil nicht leer ist.

**Remarks**

Beim Laden einer Arbeitsmappe aus einer vorhandenen Vorlagendatei können für einen Stil sowohl integrierte Zahl als auch benutzerdefiniertes Muster definiert sein. Diese Eigenschaft bestimmt, ob beim Formatieren von Werten mit dem Stil die integrierte Zahl oder das benutzerdefinierte Muster verwendet werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Legt den Standard‑Schriftartnamen für die Arbeitsmappe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


Legt die Standard‑Schriftgröße für die Arbeitsmappe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Legt den Standardwert für die horizontale Ausrichtung fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Legt den Standardwert für die vertikale Ausrichtung fest

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

