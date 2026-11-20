---
title: "FormulaParseOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt Optionen beim Parsen von Formeln dar."
type: docs
url: /de/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

Stellt Optionen beim Parsen von Formeln dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | Ob Add‑Ins in vorhandenen externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link geprüft werden. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | Definition zum Parsen benutzerdefinierter Funktionen. |
| [getLocaleDependent()](#getLocaleDependent--) | Ob die Formel lokalisierungsabhängig formatiert ist. |
| [getParse()](#getParse--) | Ob die angegebene Formel geparst wird. |
| [getR1C1Style()](#getR1C1Style--) | Ob die Formel im R1C1-Referenzstil vorliegt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | Ob Add‑Ins in vorhandenen externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link geprüft werden. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Definition zum Parsen benutzerdefinierter Funktionen. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | Ob die Formel lokalisierungsabhängig formatiert ist. |
| [setParse(boolean value)](#setParse-boolean-) | Ob die angegebene Formel geparst wird. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | Ob die Formel im R1C1-Referenzstil vorliegt. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


Ob Add‑Ins in vorhandenen externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link geprüft werden. Standard ist true (wenn die benutzerdefinierte Funktion mit einem Add‑In in vorhandenen externen Links übereinstimmt, wird sie als dieses Add‑In behandelt).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


Definition zum Parsen benutzerdefinierter Funktionen.

**Remarks**

Für einige spezielle Anforderungen, wie z. B. beim Berechnen einer benutzerdefinierten Funktion in der benutzerdefinierten Engine des Benutzers, müssen einige ihrer Parameter im Array‑Modus berechnet werden; mit dieser Eigenschaft können diese Parameter beim Parsen der Formel als Array‑Modus markiert werden. Andernfalls muss der Benutzer diese benutzerdefinierten Funktionen später mittels [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) aktualisieren, um dasselbe Ergebnis zu erhalten.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


Ob die Formel lokalisierungsformatiert ist. Standard ist false.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


Ob die angegebene Formel geparst wird. Standard ist true. Wenn false, bleibt die gegebene Formelzeichenfolge unverändert in der Zelle, bis der Benutzer andere Methoden zum Parsen aufruft oder geparste Formeldaten von anderen Vorgängen wie der Berechnung von Formeln benötigt werden.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


Ob die Formel im R1C1-Referenzstil vorliegt. Standard ist false.

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




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


Ob Add‑Ins in vorhandenen externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link geprüft werden. Standard ist true (wenn die benutzerdefinierte Funktion mit einem Add‑In in vorhandenen externen Links übereinstimmt, wird sie als dieses Add‑In behandelt).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


Definition zum Parsen benutzerdefinierter Funktionen.

**Remarks**

Für einige spezielle Anforderungen, wie z. B. beim Berechnen einer benutzerdefinierten Funktion in der benutzerdefinierten Engine des Benutzers, müssen einige ihrer Parameter im Array‑Modus berechnet werden; mit dieser Eigenschaft können diese Parameter beim Parsen der Formel als Array‑Modus markiert werden. Andernfalls muss der Benutzer diese benutzerdefinierten Funktionen später mittels [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) aktualisieren, um dasselbe Ergebnis zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


Ob die Formel lokalisierungsformatiert ist. Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


Ob die angegebene Formel geparst wird. Standard ist true. Wenn false, bleibt die gegebene Formelzeichenfolge unverändert in der Zelle, bis der Benutzer andere Methoden zum Parsen aufruft oder geparste Formeldaten von anderen Vorgängen wie der Berechnung von Formeln benötigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


Ob die Formel im R1C1-Referenzstil vorliegt. Standard ist false.

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

