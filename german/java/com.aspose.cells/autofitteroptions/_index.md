---
title: "AutoFitterOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle Optionen des automatischen Anpassungswerkzeugs dar."
type: docs
url: /de/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Stellt alle Optionen des automatischen Anpassungswerkzeugs dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Gibt an, ob die Zeilenhöhe automatisch angepasst wird, wenn Zellen in einer Zeile zusammengeführt werden. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Ermittelt den Typ der automatischen Anpassung der Zeilenhöhe für zusammengeführte Zellen. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Ermittelt den Typ der automatischen Anpassung von umgebrochenem Text. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Liefert die Standardsprache für die Bearbeitung. |
| [getForRendering()](#getForRendering--) | Gibt an, ob eine Anpassung für Renderzwecke erfolgt. |
| [getFormatStrategy()](#getFormatStrategy--) | Ermittelt die formatierte Strategie. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Ignoriert die ausgeblendeten Zeilen/Spalten. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Ermittelt die maximale Zeilenhöhe (in Punkt) beim automatischen Anpassen von Zeilen. |
| [getOnlyAuto()](#getOnlyAuto--) | Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Gibt an, ob die Zeilenhöhe automatisch angepasst wird, wenn Zellen in einer Zeile zusammengeführt werden. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Legt den Typ der automatischen Anpassung der Zeilenhöhe für zusammengeführte Zellen fest. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Legt den Typ der automatischen Anpassung von umgebrochenem Text fest. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Legt die Standardsprache für die Bearbeitung fest. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Gibt an, ob eine Anpassung für Renderzwecke erfolgt. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Legt die formatierte Strategie fest. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Ignoriert die ausgeblendeten Zeilen/Spalten. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Legt die maximale Zeilenhöhe (in Punkt) beim automatischen Anpassen von Zeilen fest. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
```


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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Gibt an, ob die Zeilenhöhe automatisch angepasst wird, wenn Zellen in einer Zeile zusammengeführt werden. Der Standardwert ist false.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft AutoFitterOptions.AutoFitMergedCellsType. Diese Eigenschaft wird 12 Monate nach Dezember 2018 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


Ermittelt den Typ der automatischen Anpassung der Zeilenhöhe für zusammengeführte Zellen.

Siehe [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignoriert standardmäßig zusammengeführte Zellen beim Anpassen der Zeilenhöhe, sodass Aspose.Cells dem Standard von MS Excel entspricht. Bitte setzen Sie diesen Typ, um die Methode des automatischen Anpassens der Zeilenhöhe für zusammengeführte Zellen zu ändern.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


Ermittelt den Typ der automatischen Anpassung von umgebrochenem Text.

Siehe [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Liefert die Standardsprache für die Bearbeitung.

Siehe [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Es kann unterschiedliche Layouts für Textabsätze anzeigen/rendern, wenn verschiedene Bearbeitungssprachen festgelegt sind. Standard ist [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


Gibt an, ob eine Anpassung für Renderzwecke erfolgt.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Ermittelt die formatierte Strategie.

Siehe [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Der Standardwert ist CellStyle aus Leistungsgründen.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Ignoriert die ausgeblendeten Zeilen/Spalten.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


Ermittelt die maximale Zeilenhöhe (in Punkt) beim automatischen Anpassen von Zeilen.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


Gibt an, ob die Zeilenhöhe automatisch angepasst wird, wenn Zellen in einer Zeile zusammengeführt werden. Der Standardwert ist false.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft AutoFitterOptions.AutoFitMergedCellsType. Diese Eigenschaft wird 12 Monate nach Dezember 2018 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


Legt den Typ der automatischen Anpassung der Zeilenhöhe für zusammengeführte Zellen fest.

Siehe [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignoriert standardmäßig zusammengeführte Zellen beim Anpassen der Zeilenhöhe, sodass Aspose.Cells dem Standard von MS Excel entspricht. Bitte setzen Sie diesen Typ, um die Methode des automatischen Anpassens der Zeilenhöhe für zusammengeführte Zellen zu ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


Legt den Typ der automatischen Anpassung von umgebrochenem Text fest.

Siehe [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Legt die Standardsprache für die Bearbeitung fest.

Siehe [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Es kann unterschiedliche Layouts für Textabsätze anzeigen/rendern, wenn verschiedene Bearbeitungssprachen festgelegt sind. Standard ist [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


Gibt an, ob eine Anpassung für Renderzwecke erfolgt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Legt die formatierte Strategie fest.

Siehe [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Der Standardwert ist CellStyle aus Leistungsgründen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


Ignoriert die ausgeblendeten Zeilen/Spalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


Legt die maximale Zeilenhöhe (in Punkt) beim automatischen Anpassen von Zeilen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist.

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

