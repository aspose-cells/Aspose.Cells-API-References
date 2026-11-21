---
title: "GridValidationType"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar datavalideringstyp."
type: docs
url: /sv/java/com.aspose.gridweb/gridvalidationtype/
---

**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```

Representerar datavalideringstyp.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | Valideringstyp för valfritt värde. |
| [BOOLEAN](#BOOLEAN) | SANT eller FALSKT |
| [CHECK_BOX](#CHECK-BOX) | Visa cellen som en kryssruta. |
| [CUSTOM](#CUSTOM) | Anpassad valideringstyp. |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | Anpassad valideringstyp, med reguljärt uttryck. |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | Anpassad JavaScript-funktionsvalidering. |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | Anpassad server‑sidig funktionsvalidering. |
| [DATE](#DATE) | Datumvalideringstyp. |
| [DATE_TIME](#DATE-TIME) | DatumTid (yyyy-MM-dd eller yyyy-MM-dd hh:mm:ss). |
| [DECIMAL](#DECIMAL) | Decimalvalideringstyp. |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | Visa rullgardinslista. |
| [FREE_LIST](#FREE-LIST) | Fri listvalideringstyp. |
| [LIST](#LIST) | Listvalideringstyp. |
| [TEXT_LENGTH](#TEXT-LENGTH) | Textlängdvalideringstyp. |
| [TIME](#TIME) | Tidvalideringstyp. |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | Heltalsvalideringstyp. |
## Metoder

| Metod | Beskrivning |
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


Valideringstyp för valfritt värde.

### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```


SANT eller FALSKT

### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```


Visa cellen som en kryssruta. Och värdet i cellen är Sant eller Falskt.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Anpassad valideringstyp.

### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```


Anpassad valideringstyp, med reguljärt uttryck.

### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```


Anpassad JavaScript-funktionsvalidering.

**Remarks**

Använd egenskapen ClientValidationFunction för att ange namn på klientvalideringsfunktionen. Funktionen bör deklareras enligt detta format:
function customValicationFunction(source, value)
Parametern "source" är cellobjektet. Parametern "value" är cellens strängvärde som ska kontrolleras. Funktionen bör returnera sant om värdet är giltigt.

### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```


Anpassad server‑sidig funktionsvalidering.

**Remarks**

Använd egenskapen CustomServerFunction för att ange server‑sidig validering. Nedan är exempel­koden:
Först definiera en klass som implementerar GridCustomServerValidation‑klassen myservervali : GridCustomServerValidation
...... sedan lägg till validering var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); sedan sätt ClientValidationFunction för att hantera klientlogik när servervalideringen misslyckas och returnera meddelandet gv.ClientValidationFunction = "ValidationErrorClientFunction"; klientfunktionen ska deklareras så här: function ValidationErrorClientFunction(cell,msg) vänligen se demosidan för en detaljerad referens

### DATE {#DATE}
```
public static final int DATE
```


Datumvalideringstyp.

### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```


DatumTid (yyyy-MM-dd eller yyyy-MM-dd hh:mm:ss).

### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Decimalvalideringstyp.

### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```


Visa rullgardinslista.

### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```


Fri listvalideringstyp.

### LIST {#LIST}
```
public static final int LIST
```


Listvalideringstyp.

### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```


Textlängdvalideringstyp.

### TIME {#TIME}
```
public static final int TIME
```


Tidvalideringstyp.

### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```


Heltalsvalideringstyp.

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

