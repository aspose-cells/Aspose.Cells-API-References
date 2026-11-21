---
title: "AbstractCalculationMonitor"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Monitor para que el usuario siga el progreso del cálculo de la fórmula."
type: docs
url: /es/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

Monitor para que el usuario siga el progreso del cálculo de la fórmula.

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | Implemente este método para realizar operaciones después de que se haya calculado una celda. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | Implemente este método para realizar operaciones antes de calcular una celda. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Obtiene el valor recién calculado de la celda. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | Obtiene el valor anterior de la celda calculada. |
| [getValueChanged()](#getValueChanged--) | Indica si el valor de la celda ha sido modificado después del cálculo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | Implemente este método para realizar operaciones al calcular fórmulas con referencias circulares. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implemente este método para realizar operaciones después de que se haya calculado una celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | Índice de la hoja a la que pertenece la celda. |
| rowIndex | int | Índice de fila de la celda |
| colIndex | int | Índice de columna de la celda |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implemente este método para realizar operaciones antes de calcular una celda.

**Remarks**

Para celdas en fórmulas de matriz, este método puede no ejecutarse porque generalmente esas celdas se calculan juntas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | Índice de la hoja a la que pertenece la celda. |
| rowIndex | int | Índice de fila de la celda |
| colIndex | int | Índice de columna de la celda |

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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Obtiene el valor recién calculado de la celda. Debe usarse solo en [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


Obtiene el valor anterior de la celda calculada. Debe usarse solo en [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) y [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


Indica si el valor de la celda ha cambiado después del cálculo. Debe usarse solo en [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


Implemente este método para realizar operaciones al calcular fórmulas con referencias circulares.

**Remarks**

En la implementación, el usuario también puede establecer el valor esperado como resultado calculado para parte/todas esas celdas, de modo que el motor de fórmulas no las calcule recursivamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator con elementos de [CalculationCell](../../com.aspose.cells/calculationcell) que representan celdas que dependen de referencias circulares. |

**Returns:**
boolean - Indica si el motor de fórmulas necesita calcular esas celdas en forma circular después de esta llamada. True para permitir que el motor de fórmulas continúe calculándolas. False para que el motor de fórmulas solo marque esas celdas como Calculated.
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

