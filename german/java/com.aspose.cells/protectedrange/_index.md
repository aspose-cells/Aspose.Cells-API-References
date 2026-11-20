---
title: "ProtectedRange"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Ein angegebener Bereich, der bearbeitet werden darf, wenn der Blattschutz aktiviert ist."
type: docs
url: /de/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

Ein angegebener Bereich, der bearbeitet werden darf, wenn der Blattschutz aktiviert ist.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Fügt diesem einen referenzierten Bereich hinzu |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Liefert alle referenzierten Bereiche. |
| [getCellArea()](#getCellArea--) | Ruft das [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) Objekt ab, das den zu schützenden Zellbereich darstellt. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Ruft den Titel des Bereichs ab. |
| [getPassword()](#getPassword--) | Stellt das Passwort zum Schutz des Bereichs dar. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort anzugeben, um auf den Bereich zuzugreifen. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Ruft den Titel des Bereichs ab. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Stellt das Passwort zum Schutz des Bereichs dar. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort anzugeben, um auf den Bereich zuzugreifen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


Fügt diesem einen referenzierten Bereich hinzu

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile. |
| startColumn | int | Die Startspalte. |
| endRow | int | Die Endzeile. |
| endColumn | int | Die Endspalte. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Liefert alle referenzierten Bereiche.

**Returns:**
com.aspose.cells.CellArea[] - Gibt alle referenzierten Bereiche zurück.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Ruft das [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) Objekt ab, das den zu schützenden Zellbereich darstellt.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Ruft den Titel des Bereichs ab. Dieser wird als Bezeichner verwendet, nicht als benannte Bereichsdefinition.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


Stellt das Passwort zum Schutz des Bereichs dar.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort anzugeben, um auf den Bereich zuzugreifen.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist.

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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ruft den Titel des Bereichs ab. Dieser wird als Bezeichner verwendet, nicht als benannte Bereichsdefinition.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Stellt das Passwort zum Schutz des Bereichs dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort anzugeben, um auf den Bereich zuzugreifen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

