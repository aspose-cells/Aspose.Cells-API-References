---
title: "GridValidationType"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Datengültigkeitstyp dar."
type: docs
url: /de/java/com.aspose.gridweb/gridvalidationtype/
---

**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```

Stellt den Datengültigkeitstyp dar.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | Validierungstyp für beliebige Werte. |
| [BOOLEAN](#BOOLEAN) | WAHR oder FALSCH |
| [CHECK_BOX](#CHECK-BOX) | Zeigt die Zelle als Kontrollkästchen an. |
| [CUSTOM](#CUSTOM) | Benutzerdefinierter Validierungstyp. |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | Benutzerdefinierter Validierungstyp, der reguläre Ausdrücke verwendet. |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | Benutzerdefinierte JavaScript-Funktionsvalidierung. |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | Benutzerdefinierte serverseitige Funktionsvalidierung. |
| [DATE](#DATE) | Datums-Validierungstyp. |
| [DATE_TIME](#DATE-TIME) | DateTime (yyyy-MM-dd oder yyyy-MM-dd hh:mm:ss). |
| [DECIMAL](#DECIMAL) | Dezimal-Validierungstyp. |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | Dropdown-Liste anzeigen. |
| [FREE_LIST](#FREE-LIST) | Freier List-Validierungstyp. |
| [LIST](#LIST) | Listen-Validierungstyp. |
| [TEXT_LENGTH](#TEXT-LENGTH) | Textlängen-Validierungstyp. |
| [TIME](#TIME) | Zeit-Validierungstyp. |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | Ganzzahl-Validierungstyp. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ANY_VALUE {#ANY-VALUE}
```
public static final int ANY_VALUE
```


Validierungstyp für beliebige Werte.

### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```


WAHR oder FALSCH

### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```


Zeigt die Zelle als Kontrollkästchen an. Und der Wert der Zelle ist Wahr oder Falsch.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Benutzerdefinierter Validierungstyp.

### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```


Benutzerdefinierter Validierungstyp, der reguläre Ausdrücke verwendet.

### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```


Benutzerdefinierte JavaScript-Funktionsvalidierung.

**Remarks**

Verwenden Sie die Eigenschaft ClientValidationFunction, um den Namen der clientseitigen Validierungsfunktion anzugeben. Die Funktion sollte in dieser Form deklariert werden:
function customValicationFunction(source, value)
Der Parameter "source" ist das Zellenobjekt. Der Parameter "value" ist der Zeichenkettenwert einer zu prüfenden Zelle. Die Funktion sollte true zurückgeben, wenn der Wert gültig ist.

### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```


Benutzerdefinierte serverseitige Funktionsvalidierung.

**Remarks**

Verwenden Sie die Eigenschaft CustomServerFunction, um die serverseitige Validierung anzugeben. Nachfolgend ist der Beispielcode:
Zuerst definieren Sie eine Klasse, die die GridCustomServerValidation-Klasse implementiert myservervali : GridCustomServerValidation
...... dann fügen Sie die Validierung hinzu var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); dann setzen Sie ClientValidationFunction, um die Client-Logik zu behandeln, wenn die Servervalidierung fehlschlägt und eine Meldung zurückgibt gv.ClientValidationFunction = "ValidationErrorClientFunction"; die Client-Funktion muss wie folgt deklariert werden: function ValidationErrorClientFunction(cell,msg) bitte prüfen Sie die Demo-Seite für eine detaillierte Referenz

### DATE {#DATE}
```
public static final int DATE
```


Datums-Validierungstyp.

### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```


DateTime (yyyy-MM-dd oder yyyy-MM-dd hh:mm:ss).

### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Dezimal-Validierungstyp.

### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```


Dropdown-Liste anzeigen.

### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```


Freier List-Validierungstyp.

### LIST {#LIST}
```
public static final int LIST
```


Listen-Validierungstyp.

### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```


Textlängen-Validierungstyp.

### TIME {#TIME}
```
public static final int TIME
```


Zeit-Validierungstyp.

### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```


Ganzzahl-Validierungstyp.

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

