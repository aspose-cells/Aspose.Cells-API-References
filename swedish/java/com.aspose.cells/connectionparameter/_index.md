---
title: "ConnectionParameter"
second_title: "Aspose.Cells för Java API-referens"
description: "Anger egenskaper för eventuella parametrar som används med externa datakopplingar. Parametrar är giltiga för ODBC- och webbfrågor."
type: docs
url: /sv/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Anger egenskaper för eventuella parametrar som används med externa datakopplingar. Parametrar är giltiga för ODBC- och webbfrågor.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Cellreferens som anger vilken cells värde som ska användas för frågeparametern. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Namnet på parametern. |
| [getPrompt()](#getPrompt--) | Uppmaningssträng för parametern. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Flagga som indikerar om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. |
| [getSqlType()](#getSqlType--) | SQL-datatyp för parametern. |
| [getType()](#getType--) | Typ av parameter som används. |
| [getValue()](#getValue--) | Icke-heltaligt numeriskt värde, heltalsvärde, strängvärde eller booleskt värde att använda som frågeparameter. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | Cellreferens som anger vilken cells värde som ska användas för frågeparametern. |
| [setName(String value)](#setName-java.lang.String-) | Namnet på parametern. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | Uppmaningssträng för parametern. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | Flagga som indikerar om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. |
| [setSqlType(int value)](#setSqlType-int-) | SQL-datatyp för parametern. |
| [setType(int value)](#setType-int-) | Typ av parameter som används. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Icke-heltaligt numeriskt värde, heltalsvärde, strängvärde eller booleskt värde att använda som frågeparameter. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Cellreferens som anger vilken cells värde som ska användas för frågeparametern. Används endast när parameterType är cell.

**Returns:**
java.lang.String
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


Namnet på parametern.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Uppmaningssträng för parametern. Presenteras för kalkylbladsanvändaren tillsammans med inmatnings‑UI för att samla in parametervärdet innan extern data uppdateras. Används endast när parameterType = prompt.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Flagga som indikerar om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. Om true, uppdateras extern data med det nya parametervärdet varje gång en förändring sker. Om false, uppdateras extern data endast när användaren begär det, eller när någon annan händelse triggar en uppdatering (t.ex. arbetsboken öppnas).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


SQL-datatyp för parametern. Endast giltig för ODBC‑källor.

Se [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Typ av parameter som används. Om parameterType=value, används värdet från boolean, double, integer eller string. I detta fall förväntas endast ett av \{boolean, double, integer, or string\} specificeras.

Se [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Icke-heltaligt numeriskt värde, heltalsvärde, strängvärde eller booleskt värde att använda som frågeparameter. Används endast när parameterType är value.

**Returns:**
java.lang.Object
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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


Cellreferens som anger vilken cells värde som ska användas för frågeparametern. Används endast när parameterType är cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Namnet på parametern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


Uppmaningssträng för parametern. Presenteras för kalkylbladsanvändaren tillsammans med inmatnings‑UI för att samla in parametervärdet innan extern data uppdateras. Används endast när parameterType = prompt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


Flagga som indikerar om frågan ska uppdateras automatiskt när innehållet i en cell som tillhandahåller parametervärdet ändras. Om true, uppdateras extern data med det nya parametervärdet varje gång en förändring sker. Om false, uppdateras extern data endast när användaren begär det, eller när någon annan händelse triggar en uppdatering (t.ex. arbetsboken öppnas).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


SQL-datatyp för parametern. Endast giltig för ODBC‑källor.

Se [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Typ av parameter som används. Om parameterType=value, används värdet från boolean, double, integer eller string. I detta fall förväntas endast ett av \{boolean, double, integer, or string\} specificeras.

Se [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Icke-heltaligt numeriskt värde, heltalsvärde, strängvärde eller booleskt värde att använda som frågeparameter. Används endast när parameterType är value.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

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

