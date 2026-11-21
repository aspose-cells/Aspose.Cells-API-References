---
title: "PivotFieldGroupOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones para la configuración de agrupación de campos de tabla dinámica."
type: docs
url: /es/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Opciones para la configuración de agrupación de campos de tabla dinámica.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // Group the first row field (a date field) by months and quarters
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartDate(new DateTime(2008, 1, 1));
         options.setEndDate(new DateTime(2008, 9, 5));
         options.setGroupTypes(new /*PivotGroupByType*/int[] { PivotGroupByType.MONTHS, PivotGroupByType.QUARTERS });
         pt.getRowFields().get(0).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputGroupPivotFieldsInPivotTable.xlsx");
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | Obtiene los elementos de grupo discretos. |
| [getEndDate()](#getEndDate--) | Obtiene el valor final del rango de agrupación. |
| [getEndNumber()](#getEndNumber--) | Obtiene el valor final del rango de agrupación. |
| [getGroupType()](#getGroupType--) | Obtiene el tipo de agrupación para el pivot field. |
| [getGroupTypes()](#getGroupTypes--) | Obtiene el tipo de agrupación para el pivot field. |
| [getInterval()](#getInterval--) | Obtiene el tamaño del intervalo para cada grupo. |
| [getNewPivotField()](#getNewPivotField--) | Obtiene un valor que indica si se deben crear nuevos pivot fields después del agrupamiento. |
| [getStartDate()](#getStartDate--) | Obtiene el valor inicial del rango de agrupación. |
| [getStartNumber()](#getStartNumber--) | Obtiene el valor inicial del rango de agrupación. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Obtiene un valor que indica si el valor final se determina automáticamente. |
| [isAutoStart()](#isAutoStart--) | Obtiene un valor que indica si el valor inicial se determina automáticamente. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Establece un valor que indica si el valor final se determina automáticamente. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Establece un valor que indica si el valor inicial se determina automáticamente. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | Establece los elementos de grupo discretos. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Establece el valor final del rango de agrupación. |
| [setEndNumber(double value)](#setEndNumber-double-) | Establece el valor final del rango de agrupación. |
| [setGroupType(int value)](#setGroupType-int-) | Establece el tipo de agrupación para el pivot field. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Establece el tipo de agrupación para el pivot field. |
| [setInterval(double value)](#setInterval-double-) | Establece el tamaño del intervalo para cada grupo. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Establece un valor que indica si se deben crear nuevos pivot fields después del agrupamiento. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Establece el valor inicial del rango de agrupación. |
| [setStartNumber(double value)](#setStartNumber-double-) | Establece el valor inicial del rango de agrupación. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


Obtiene los elementos de grupo discretos.

**Remarks**

Si esta propiedad está establecida,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Obtiene el valor final del rango de agrupación.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Obtiene el valor final del rango de agrupación.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Obtiene el tipo de agrupación para el campo dinámico. Sólo para agrupar campos dinámicos de fecha y hora.

Ver [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         //init
         PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
         // Group by year and month together
         /*PivotGroupByType*/int pivotGroupByType = pivotFieldGroupOptions.getGroupType();
         pivotGroupByType = PivotGroupByType.YEARS | PivotGroupByType.MONTHS;
         pivotFieldGroupOptions.setGroupType(pivotGroupByType);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


Obtiene el tipo de agrupación para el pivot field.

Ver [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

El orden en esta propiedad será ignorado. Al especificar varios tipos de grupo, los campos de grupo base se insertarán en orden ascendente y el campo de grupo se mostrará en la región de fila/columna en orden descendente (Años \\u922b?Trimestres \\u922b?Meses \\u922b?Días \\u922b?Horas \\u922b?Minutos \\u922b?Segundos).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Obtiene el tamaño del intervalo para cada grupo.

**Remarks**

Sólo para grupos de número y días.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Obtiene un valor que indica si se deben crear nuevos pivot fields después del agrupamiento.

**Remarks**

Si no se establece explícitamente, el valor predeterminado es false para el agrupamiento numérico y true para el agrupamiento de fecha y hora, true para el grupo discreto. Sólo funciona para el primer nuevo campo dinámico de grupo del campo base.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Obtiene el valor inicial del rango de agrupación.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Obtiene el valor inicial del rango de agrupación.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


Obtiene un valor que indica si el valor final se determina automáticamente.

**Remarks**

Si [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) o [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) está establecido, esta propiedad será false.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Obtiene un valor que indica si el valor inicial se determina automáticamente.

**Remarks**

Si [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) o [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) está establecido, esta propiedad será false.

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




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


Establece un valor que indica si el valor final se determina automáticamente.

**Remarks**

Si [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) o [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) está establecido, esta propiedad será false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Establece un valor que indica si el valor inicial se determina automáticamente.

**Remarks**

Si [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) o [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) está establecido, esta propiedad será false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


Establece los elementos de grupo discretos.

**Remarks**

Si esta propiedad está establecida,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Establece el valor final del rango de agrupación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Establece el valor final del rango de agrupación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Establece el tipo de agrupación para el campo dinámico. Sólo para agrupar campos dinámicos de fecha y hora.

Ver [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Establece el tipo de agrupación para el pivot field.

Ver [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

El orden en esta propiedad será ignorado. Al especificar varios tipos de grupo, los campos de grupo base se insertarán en orden ascendente y el campo de grupo se mostrará en la región de fila/columna en orden descendente (Años \\u922b?Trimestres \\u922b?Meses \\u922b?Días \\u922b?Horas \\u922b?Minutos \\u922b?Segundos).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Establece el tamaño del intervalo para cada grupo.

**Remarks**

Sólo para grupos de número y días.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Establece un valor que indica si se deben crear nuevos pivot fields después del agrupamiento.

**Remarks**

Si no se establece explícitamente, el valor predeterminado es false para el agrupamiento numérico y true para el agrupamiento de fecha y hora, true para el grupo discreto. Sólo funciona para el primer nuevo campo dinámico de grupo del campo base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Establece el valor inicial del rango de agrupación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Establece el valor inicial del rango de agrupación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

