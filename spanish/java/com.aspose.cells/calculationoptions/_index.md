---
title: "CalculationOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa opciones de cálculo."
type: docs
url: /es/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Representa opciones de cálculo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | El tamaño de la pila para calcular celdas de forma recursiva. |
| [getCalculationMonitor()](#getCalculationMonitor--) | El monitor para que el usuario siga el progreso del cálculo de fórmulas. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Especifica la codificación utilizada para codificar/decodificar caracteres al calcular fórmulas. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [getIgnoreError()](#getIgnoreError--) | Indica si los errores encontrados al calcular fórmulas deben ser ignorados. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Especifica las fuentes de datos para los enlaces externos utilizados en fórmulas. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Especifica la estrategia para procesar la precisión del cálculo. |
| [getRecursive()](#getRecursive--) | Indica si se deben calcular recursivamente las celdas dependientes al calcular una celda que depende de otras celdas. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Indica si las fórmulas de matriz dinámica deben actualizarse antes de calcular fórmulas. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Indica si el usuario ha especificado explícitamente el comportamiento de actualizar las fórmulas de matriz dinámica antes de calcular fórmulas específicas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | El tamaño de la pila para calcular celdas de forma recursiva. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | El monitor para que el usuario siga el progreso del cálculo de fórmulas. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Especifica la codificación utilizada para codificar/decodificar caracteres al calcular fórmulas. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indica si los errores encontrados al calcular fórmulas deben ser ignorados. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Especifica las fuentes de datos para los enlaces externos utilizados en fórmulas. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Especifica la estrategia para procesar la precisión del cálculo. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Indica si se deben calcular recursivamente las celdas dependientes al calcular una celda que depende de otras celdas. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Indica si las fórmulas de matriz dinámica deben actualizarse antes de calcular fórmulas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
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
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


El tamaño de la pila para calcular celdas de forma recursiva. El valor predeterminado es 200.

**Remarks**

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


El monitor para que el usuario siga el progreso del cálculo de fórmulas.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Especifica las fuentes de datos para los enlaces externos utilizados en fórmulas.

**Remarks**

Al igual que [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), aquí puede especificar fuentes de datos para los enlaces externos utilizados en fórmulas que se van a calcular, especialmente los que se usan en la función INDIRECT. Para esos enlaces externos usados en la función INDIRECT, no se consideran parte de los enlaces externos del libro y no pueden ser actualizados por [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). La coincidencia de esos libros con enlaces externos se determina mediante [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) y [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Por lo tanto, asegúrese de que [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) haya sido especificado con el valor adecuado (generalmente debe ser el mismo que el correspondiente [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) para cada libro, de modo que puedan enlazarse como se espera.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Especifica la estrategia para procesar la precisión del cálculo.

Ver [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


Indica si las fórmulas de matriz dinámica deben actualizarse antes de calcular fórmulas.

**Remarks**

Si esta propiedad se ha especificado explícitamente, entonces el valor especificado se usará para determinar si se actualizan las fórmulas de matrices dinámicas. De lo contrario ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) es false), el valor predeterminado depende del tipo de fórmulas que deben calcularse: para calcular fórmulas del libro, como [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), esta propiedad se considerará true. En otros casos, como [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) o [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), esta propiedad se considerará false.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


Indica si el usuario ha especificado explícitamente el comportamiento de actualizar las fórmulas de matriz dinámica antes de calcular fórmulas específicas.

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




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


El tamaño de la pila para calcular celdas de forma recursiva. El valor predeterminado es 200.

**Remarks**

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


El monitor para que el usuario siga el progreso del cálculo de fórmulas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Especifica las fuentes de datos para los enlaces externos utilizados en fórmulas.

**Remarks**

Al igual que [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), aquí puede especificar fuentes de datos para los enlaces externos utilizados en fórmulas que se van a calcular, especialmente los que se usan en la función INDIRECT. Para esos enlaces externos usados en la función INDIRECT, no se consideran parte de los enlaces externos del libro y no pueden ser actualizados por [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). La coincidencia de esos libros con enlaces externos se determina mediante [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) y [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Por lo tanto, asegúrese de que [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) haya sido especificado con el valor adecuado (generalmente debe ser el mismo que el correspondiente [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) para cada libro, de modo que puedan enlazarse como se espera.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Especifica la estrategia para procesar la precisión del cálculo.

Ver [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


Indica si las fórmulas de matriz dinámica deben actualizarse antes de calcular fórmulas.

**Remarks**

Si esta propiedad se ha especificado explícitamente, entonces el valor especificado se usará para determinar si se actualizan las fórmulas de matrices dinámicas. De lo contrario ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) es false), el valor predeterminado depende del tipo de fórmulas que deben calcularse: para calcular fórmulas del libro, como [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), esta propiedad se considerará true. En otros casos, como [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) o [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), esta propiedad se considerará false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

