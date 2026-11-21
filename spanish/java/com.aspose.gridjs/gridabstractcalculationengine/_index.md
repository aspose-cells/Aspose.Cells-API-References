---
title: "GridAbstractCalculationEngine"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells."
type: docs
url: /es/java/com.aspose.gridjs/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.

**Remarks**

El usuario no debe modificar ninguna parte del Workbook directamente en esta implementación (excepto el resultado calculado de la función personalizada, que puede establecerse mediante la propiedad GridCalculationData.CalculatedValue). De lo contrario, podrían producirse resultados inesperados o una Excepción. Si el usuario necesita cambiar datos distintos al resultado calculado en la implementación para algunas funciones personalizadas, por ejemplo, modificar la fórmula de una celda, el estilo, etc., debe recopilar esos datos en esta implementación y modificarlos fuera del ámbito del cálculo de fórmulas.

**Example**

```
          class MyEngine extends GridAbstractCalculationEngine
         {
             public /*override*/ void calculate(GridCalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {   
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof GridReferredArea)
                         {
                             GridReferredArea ra = (GridReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridjs.GridCalculationData-) | Calcula una función con los datos proporcionados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```


### calculate(GridCalculationData data) {#calculate-com.aspose.gridjs.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


Calcula una función con los datos proporcionados.

**Remarks**

El usuario debe establecer el valor calculado para los datos dados de todas las funciones (incluyendo las funciones nativas de Excel) que desea calcular por sí mismo en esta implementación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridjs/gridcalculationdata) | Los datos necesarios para calcular la función, como el nombre de la función, los parámetros, etc. |

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

