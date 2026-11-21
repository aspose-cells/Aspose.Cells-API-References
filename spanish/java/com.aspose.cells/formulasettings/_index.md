---
title: "FormulaSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Configuraciones de fórmulas y cálculo."
type: docs
url: /es/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Configuraciones de fórmulas y cálculo.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Indica si la aplicación debe realizar un cálculo completo cuando se abre el libro de trabajo. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Indica si se debe recalcular el libro de trabajo antes de guardar el documento, cuando está en modo de cálculo manual. |
| [getCalculationId()](#getCalculationId--) | Especifica la versión del motor de cálculo utilizado para calcular los valores en el libro de trabajo. |
| [getCalculationMode()](#getCalculationMode--) | Obtiene el modo de cálculo del libro de trabajo en MS Excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Indica si se debe habilitar la cadena de cálculo para fórmulas. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Indica si se debe habilitar el cálculo iterativo para resolver referencias circulares. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Indica si calcula todas las fórmulas cada vez que se desencadena un cálculo. |
| [getMaxChange()](#getMaxChange--) | El cambio máximo para resolver una referencia circular. |
| [getMaxIteration()](#getMaxIteration--) | El número máximo de iteraciones para resolver una referencia circular. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Indica si la precisión del resultado calculado se establece tal como se muestra al calcular fórmulas. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Indica si se deben conservar los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | Indica si la aplicación debe realizar un cálculo completo cuando se abre el libro de trabajo. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | Indica si se debe recalcular el libro de trabajo antes de guardar el documento, cuando está en modo de cálculo manual. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | Especifica la versión del motor de cálculo utilizado para calcular los valores en el libro de trabajo. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Establece el modo de cálculo del libro de trabajo en MS Excel. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | Indica si se debe habilitar la cadena de cálculo para fórmulas. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | Indica si se debe habilitar el cálculo iterativo para resolver referencias circulares. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | Indica si calcula todas las fórmulas cada vez que se desencadena un cálculo. |
| [setMaxChange(double value)](#setMaxChange-double-) | El cambio máximo para resolver una referencia circular. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | El número máximo de iteraciones para resolver una referencia circular. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Indica si la precisión del resultado calculado se establece tal como se muestra al calcular fórmulas. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Indica si se deben conservar los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Indica si la aplicación debe realizar un cálculo completo cuando se abre el libro de trabajo.

**Remarks**

Esta propiedad solo sirve para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Indica si se debe recalcular el libro de trabajo antes de guardar el documento, cuando está en modo de cálculo manual.

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Especifica la versión del motor de cálculo utilizado para calcular los valores en el libro de trabajo.

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. En el caso de ms excel, si el valor de esta propiedad es menor que el identificador del motor de recálculo asociado con la aplicación que abre el archivo resultante, la aplicación recalculará los resultados de todas las fórmulas en este libro de trabajo inmediatamente después de cargar el archivo. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


Obtiene el modo de cálculo del libro de trabajo en MS Excel.

Ver [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones del usuario, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué modo se haya establecido para esta propiedad. Si el usuario necesita calcular fórmulas, por favor siempre invoque los métodos en diferentes objetos según el requisito: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


Indica si se debe habilitar la cadena de cálculo para fórmulas. El valor predeterminado es false.

**Remarks**

Cuando hay muchas fórmulas en el libro de trabajo y el usuario necesita calcularlas repetidamente modificando solo una pequeña parte de ellas, puede ser útil para el rendimiento habilitar la cadena de cálculo. Por otro lado, si la cadena está habilitada, mantener el modelo de cadena requiere memoria adicional, y también requiere un poco más de tiempo de CPU para algunas otras operaciones, como cambiar el valor o las fórmulas de una celda. Después de cambiar esta propiedad de false a true, la cadena de cálculo se analizará y construirá en el momento del primer cálculo del libro de trabajo, por lo que el tiempo requerido para el primer cálculo puede ser mayor que el cálculo normal sin cadena.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Indica si se debe habilitar el cálculo iterativo para resolver referencias circulares.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Indica si calcula todas las fórmulas cada vez que se desencadena un cálculo.

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


El cambio máximo para resolver una referencia circular.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


El número máximo de iteraciones para resolver una referencia circular.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Indica si la precisión del resultado calculado se establece tal como se muestra al calcular fórmulas.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Indica si se deben preservar los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Generalmente esos espacios y saltos de línea son solo para fines visuales; preservarlos o no no afecta el resultado calculado. Por consideraciones de rendimiento, si no hay un requisito especial, es mejor no preservarlos al procesar fórmulas.

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


Indica si la aplicación debe realizar un cálculo completo cuando se abre el libro de trabajo.

**Remarks**

Esta propiedad solo sirve para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


Indica si se debe recalcular el libro de trabajo antes de guardar el documento, cuando está en modo de cálculo manual.

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


Especifica la versión del motor de cálculo utilizado para calcular los valores en el libro de trabajo.

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. En el caso de ms excel, si el valor de esta propiedad es menor que el identificador del motor de recálculo asociado con la aplicación que abre el archivo resultante, la aplicación recalculará los resultados de todas las fórmulas en este libro de trabajo inmediatamente después de cargar el archivo. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


Establece el modo de cálculo del libro de trabajo en MS Excel.

Ver [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones del usuario, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué modo se haya establecido para esta propiedad. Si el usuario necesita calcular fórmulas, por favor siempre invoque los métodos en diferentes objetos según el requisito: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


Indica si se debe habilitar la cadena de cálculo para fórmulas. El valor predeterminado es false.

**Remarks**

Cuando hay muchas fórmulas en el libro de trabajo y el usuario necesita calcularlas repetidamente modificando solo una pequeña parte de ellas, puede ser útil para el rendimiento habilitar la cadena de cálculo. Por otro lado, si la cadena está habilitada, mantener el modelo de cadena requiere memoria adicional, y también requiere un poco más de tiempo de CPU para algunas otras operaciones, como cambiar el valor o las fórmulas de una celda. Después de cambiar esta propiedad de false a true, la cadena de cálculo se analizará y construirá en el momento del primer cálculo del libro de trabajo, por lo que el tiempo requerido para el primer cálculo puede ser mayor que el cálculo normal sin cadena.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


Indica si se debe habilitar el cálculo iterativo para resolver referencias circulares.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


Indica si calcula todas las fórmulas cada vez que se desencadena un cálculo.

**Remarks**

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante, de modo que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


El cambio máximo para resolver una referencia circular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


El número máximo de iteraciones para resolver una referencia circular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Indica si la precisión del resultado calculado se establece tal como se muestra al calcular fórmulas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Indica si se deben preservar los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Generalmente esos espacios y saltos de línea son solo para fines visuales; preservarlos o no no afecta el resultado calculado. Por consideraciones de rendimiento, si no hay un requisito especial, es mejor no preservarlos al procesar fórmulas.

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

