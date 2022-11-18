---
title: ConnectionParameter
second_title: Aspose.Cells for Java API Reference
description: Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.
type: docs
weight: 113
url: /java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Specifies properties about any parameters used with external data connections Parameters are valid for ODBC and web queries.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Cell reference indicating which cell's value to use for the query parameter. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | The name of the parameter. |
| [getPrompt()](#getPrompt--) | Prompt string for the parameter. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. |
| [getSqlType()](#getSqlType--) | SQL data type of the parameter. |
| [getType()](#getType--) | Type of parameter used. |
| [getValue()](#getValue--) | Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | For the description of this property, please see \#getCellReference().getCellReference() |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see \#getName().getName() |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | For the description of this property, please see \#getPrompt().getPrompt() |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | For the description of this property, please see \#getRefreshOnChange().getRefreshOnChange() |
| [setSqlType(int value)](#setSqlType-int-) | For the description of this property, please see \#getSqlType().getSqlType() |
| [setType(int value)](#setType-int-) | For the description of this property, please see \#getType().getType() |
| [setValue(Object value)](#setValue-java.lang.Object-) | For the description of this property, please see \#getValue().getValue() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Cell reference indicating which cell's value to use for the query parameter. Used only when parameterType is cell.

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


The name of the parameter.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Prompt string for the parameter. Presented to the spreadsheet user along with input UI to collect the parameter value before refreshing the external data. Used only when parameterType = prompt.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Flag indicating whether the query should automatically refresh when the contents of a cell that provides the parameter value changes. If true, then external data is refreshed using the new parameter value every time there's a change. If false, then external data is only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


SQL data type of the parameter. Only valid for ODBC sources.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Type of parameter used. If the parameterType=value, then the value from boolean, double, integer, or string will be used. In this case, it is expected that only one of \{boolean, double, integer, or string\} will be specified.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Non-integer numeric value,Integer value,String value or Boolean value to use as the query parameter. Used only when parameterType is value.

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


For the description of this property, please see \#getCellReference().getCellReference()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see \#getName().getName()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


For the description of this property, please see \#getPrompt().getPrompt()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


For the description of this property, please see \#getRefreshOnChange().getRefreshOnChange()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


For the description of this property, please see \#getSqlType().getSqlType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


For the description of this property, please see \#getType().getType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


For the description of this property, please see \#getValue().getValue()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

