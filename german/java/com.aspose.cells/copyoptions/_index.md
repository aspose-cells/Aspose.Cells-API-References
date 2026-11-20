---
title: "CopyOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Kopieroptionen dar."
type: docs
url: /de/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Stellt die Kopieroptionen dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions Konstruktor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Gibt an, ob die Spaltenbreite in Zeichen als Einheit kopiert wird. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | Wenn die Formel für das Ziel nicht gültig ist, werden nur Werte kopiert. |
| [getCopyNames()](#getCopyNames--) | Gibt an, ob die Namen kopiert werden. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Gibt an, ob Bereiche erweitert werden, wenn der Bereich in einen angrenzenden Bereich kopiert wird. |
| [getKeepMacros()](#getKeepMacros--) | Gibt an, ob Makros beibehalten werden; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | Gibt an, ob auf das Zielarbeitsblatt verwiesen werden soll, wenn das referenzierte Arbeitsblatt nicht kopiert wird. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Gibt an, ob die Spaltenbreite in Zeichen als Einheit kopiert wird. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | Wenn die Formel für das Ziel nicht gültig ist, werden nur Werte kopiert. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | Gibt an, ob die Namen kopiert werden. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Gibt an, ob Bereiche erweitert werden, wenn der Bereich in einen angrenzenden Bereich kopiert wird. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Gibt an, ob Makros beibehalten werden; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | Gibt an, ob auf das Zielarbeitsblatt verwiesen werden soll, wenn das referenzierte Arbeitsblatt nicht kopiert wird. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


CopyOptions Konstruktor.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Gibt an, ob die Spaltenbreite in Zeichen als Einheit kopiert wird.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


Wenn die Formel für das Ziel nicht gültig ist, werden nur Werte kopiert.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


Gibt an, ob die Namen kopiert werden.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Gibt an, ob Bereiche erweitert werden, wenn der Bereich in einen angrenzenden Bereich kopiert wird.

**Remarks**

Wenn es true ist, wird nur der Bereich des Hyperlinks erweitert, ohne einen neuen Hyperlink hinzuzufügen, wenn Hyperlinks in benachbarte Zeilen kopiert werden.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Gibt an, ob Makros beibehalten werden;

**Remarks**

Nur beim Kopieren der Arbeitsmappe.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist.

**Remarks**

Der Standardwert ist false, es funktioniert wie MS Excel. Zum Beispiel: Wenn ein Diagramm mit der Datenquelle "sheet1!A1:B10" von Arbeitsblatt "sheet1 zu einem anderen Arbeitsblatt "sheet2" kopiert wird, wird die Datenquelle zu "sheet2!A1:B10" geändert.

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. In einigen Situationen kann der Benutzer jedoch benötigen, dass die kopierten Formeln auf Arbeitsblätter mit demselben Namen in derselben Arbeitsmappe verweisen, zum Beispiel wenn diese Arbeitsblätter bereits vor diesem Kopiervorgang kopiert wurden; dann sollte diese Eigenschaft auf true gesetzt bleiben.

**Remarks**

Der Standardwert ist true.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


Gibt an, ob auf das Zielarbeitsblatt verwiesen werden soll, wenn das referenzierte Arbeitsblatt nicht kopiert wird.

**Remarks**

Funktioniert nur beim Kopieren von Bereich oder Arbeitsblatt aus einer anderen Arbeitsmappe.

**Returns:**
boolean
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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


Gibt an, ob die Spaltenbreite in Zeichen als Einheit kopiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


Wenn die Formel für das Ziel nicht gültig ist, werden nur Werte kopiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


Gibt an, ob die Namen kopiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


Gibt an, ob Bereiche erweitert werden, wenn der Bereich in einen angrenzenden Bereich kopiert wird.

**Remarks**

Wenn es true ist, wird nur der Bereich des Hyperlinks erweitert, ohne einen neuen Hyperlink hinzuzufügen, wenn Hyperlinks in benachbarte Zeilen kopiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


Gibt an, ob Makros beibehalten werden;

**Remarks**

Nur beim Kopieren der Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist.

**Remarks**

Der Standardwert ist false, es funktioniert wie MS Excel. Zum Beispiel: Wenn ein Diagramm mit der Datenquelle "sheet1!A1:B10" von Arbeitsblatt "sheet1 zu einem anderen Arbeitsblatt "sheet2" kopiert wird, wird die Datenquelle zu "sheet2!A1:B10" geändert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. In einigen Situationen kann der Benutzer jedoch benötigen, dass die kopierten Formeln auf Arbeitsblätter mit demselben Namen in derselben Arbeitsmappe verweisen, zum Beispiel wenn diese Arbeitsblätter bereits vor diesem Kopiervorgang kopiert wurden; dann sollte diese Eigenschaft auf true gesetzt bleiben.

**Remarks**

Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


Gibt an, ob auf das Zielarbeitsblatt verwiesen werden soll, wenn das referenzierte Arbeitsblatt nicht kopiert wird.

**Remarks**

Funktioniert nur beim Kopieren von Bereich oder Arbeitsblatt aus einer anderen Arbeitsmappe.

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

