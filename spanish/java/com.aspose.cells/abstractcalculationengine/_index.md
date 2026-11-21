---
title: "AbstractCalculationEngine"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells."
type: docs
url: /es/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.

**Remarks**

El usuario no debe modificar ninguna parte del Workbook directamente en esta implementación (excepto el resultado calculado de la función personalizada, que puede establecerse mediante la propiedad CalculationData.CalculatedValue). De lo contrario, pueden producirse resultados inesperados o una Exception. Si el usuario necesita cambiar datos distintos al resultado calculado en la implementación para algunas funciones personalizadas, por ejemplo, cambiar la fórmula de una celda, el estilo, etc., el usuario debe recopilar esos datos en esta implementación y modificarlos fuera del alcance del cálculo de la fórmula.

**Example**

```
         class MyEngine extends AbstractCalculationEngine
         {
             public /*override*/ void calculate(CalculationData data)
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
                         if (pv instanceof ReferredArea)
                         {
                             ReferredArea ra = (ReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
         Workbook wb = new Workbook("custom_calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCustomEngine(new MyEngine());
         wb.calculateFormula(opts);
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Calcula una función con los datos proporcionados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Indica si se debe forzar que la función dada se recalcule siempre al calcular fórmulas compartidas. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Indica si las funciones incorporadas que han sido soportadas por el motor incorporado deben ser verificadas y procesadas por esta implementación. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Indica si este motor necesita que el parámetro se calcule en modo de matriz. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Indica si este motor necesita el texto literal del parámetro al realizar un cálculo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Omite el cálculo de toda la fórmula que hace referencia a la función que se está evaluando actualmente. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationEngine() {#AbstractCalculationEngine--}
```
public AbstractCalculationEngine()
```


### calculate(CalculationData data) {#calculate-com.aspose.cells.CalculationData-}
```
public abstract void calculate(CalculationData data)
```


Calcula una función con los datos proporcionados.

**Remarks**

El usuario debe establecer el valor calculado para los datos dados de todas las funciones (incluyendo las funciones nativas de Excel) que desea calcular por sí mismo en esta implementación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | los datos requeridos para calcular la función, como el nombre de la función, los parámetros, etc. |

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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Indica si se debe forzar que la función dada se recalcule siempre al calcular fórmulas compartidas.

**Remarks**

Para fórmulas compartidas, varias celdas comparten la misma función. Si los parámetros de la función también permanecen iguales para esas celdas, generalmente esa función solo necesita calcularse una vez. Por lo tanto, por consideraciones de rendimiento solo calculamos este tipo de función una vez también ([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) se llama solo una vez, en lugar de ser llamado repetidamente para cada celda). Sin embargo, para la implementación personalizada del usuario, puede que la función, especialmente la función personalizada, necesite calcularse de manera diferente para distintas celdas. En ese caso, el usuario debe sobrescribir este método para que devuelva true para la función. Y para [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-), el [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) proporcionado puede haber sido inicializado con el valor en caché del cálculo anterior.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionName | java.lang.String | nombre de la función. Generalmente es el nombre de la función personalizada. Si [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) es true, entonces también se verificarán las funciones incorporadas aquí. |

**Returns:**
booleano - true si la función especificada necesita recalcularse siempre.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}
```
public boolean getProcessBuiltInFunctions()
```


Indica si las funciones incorporadas que han sido soportadas por el motor incorporado deben ser verificadas y procesadas por esta implementación. El valor predeterminado es false.

**Remarks**

Si el usuario necesita cambiar la lógica de cálculo de algunas funciones incorporadas, esta propiedad debe establecerse como true. De lo contrario, por consideraciones de rendimiento, deje esta propiedad como false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isParamArrayModeRequired() {#isParamArrayModeRequired--}
```
public boolean isParamArrayModeRequired()
```


Indica si este motor necesita que el parámetro se calcule en modo de matriz. El valor predeterminado es false. Si se requiere [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) al calcular funciones personalizadas y el usuario no ha actualizado la definición para ellas (mediante [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-)), esta propiedad debe establecerse como true.

**Remarks**

Si este motor de cálculo personalizado necesita que el parámetro se calcule en modo de matriz, se requerirán más pilas para almacenar en caché el árbol de parámetros y el método Calculate() puede ser llamado recursivamente para calcular el valor del parámetro. Por consideraciones de rendimiento, mantenga esta propiedad con el valor predeterminado (false) si no hay requisitos especiales.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Indica si este motor necesita el texto literal del parámetro al realizar un cálculo. El valor predeterminado es false.

**Remarks**

Si este motor de cálculo personalizado necesita el texto literal del parámetro, se requerirán más pilas para almacenar en caché el texto literal de los parámetros y el método Calculate() puede ser llamado recursivamente para calcular el valor del parámetro. En general, el texto literal no es necesario para calcular fórmulas y esta propiedad debe mantenerse como false para la mayoría de las implementaciones para obtener un mejor rendimiento.

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




### skipCalculation() {#skipCalculation--}
```
public void skipCalculation()
```


Omite el cálculo de toda la fórmula que hace referencia a la función que se está evaluando actualmente.

**Remarks**

Este método puede ser invocado en la implementación de [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) para omitir el cálculo de toda la fórmula y el valor original de la fórmula se mantendrá sin cambios.

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

