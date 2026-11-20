---
title: "AbstractCalculationEngine"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет пользовательский движок вычислений, расширяющий движок вычислений по умолчанию в Aspose.Cells."
type: docs
url: /ru/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Представляет пользовательский движок вычислений для расширения движка вычислений по умолчанию в Aspose.Cells.

**Remarks**

Пользователь не должен изменять любую часть Workbook напрямую в этой реализации (за исключением вычисленного результата пользовательской функции, который можно задать через свойство CalculationData.CalculatedValue). В противном случае могут возникнуть неожиданные результаты или исключения. Если пользователю необходимо изменить другие данные, кроме вычисленного результата, в реализации для некоторых пользовательских функций, например, изменить формулу ячейки, стиль и т.д., пользователь должен собрать эти данные в этой реализации и изменить их вне области вычисления формулы.

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
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Вычисляет одну функцию с заданными данными. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Определяет, следует ли принудительно пересчитывать данную функцию каждый раз при вычислении общих формул. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Определяет, должны ли встроенные функции, поддерживаемые встроенным движком, проверяться и обрабатываться этой реализацией. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Указывает, требуется ли этому движку вычислять параметр в режиме массива. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Указывает, требуется ли этому движку буквальный текст параметра во время вычисления. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Пропускает вычисление всей формулы, которая ссылается на функцию, находящуюся в текущей оценке. |
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


Вычисляет одну функцию с заданными данными.

**Remarks**

Пользователь должен установить вычисленное значение для заданных данных для всех функций (включая встроенные функции Excel), которые он хочет вычислять самостоятельно в этой реализации.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | необходимые данные для вычисления функции, такие как имя функции, параметры и т.д. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Определяет, следует ли принудительно пересчитывать данную функцию каждый раз при вычислении общих формул.

**Remarks**

Для общих формул несколько ячеек используют одну и ту же функцию. Если параметры функции также одинаковы для этих ячеек, обычно эту функцию требуется вычислять только один раз. Поэтому с точки зрения производительности мы также вычисляем такой тип функции один раз ([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) вызывается только один раз, а не повторяется для каждой ячейки). Однако в пользовательской реализации функция, особенно пользовательская функция, может потребоваться вычислять по‑разному для разных ячеек. В этом случае пользователь должен переопределить этот метод, чтобы он возвращал true для функции. И для [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) заданный [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) может быть инициализирован кэшированным значением предыдущего вычисления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| functionName | java.lang.String | имя функции. Обычно это имя пользовательской функции. Если [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) равно true, то встроенные функции также будут проверяться здесь. |

**Returns:**
логическое значение — true, если указанную функцию необходимо пересчитывать каждый раз.
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


Определяет, должны ли встроенные функции, поддерживаемые встроенным движком, проверяться и обрабатываться этой реализацией. По умолчанию false.

**Remarks**

Если пользователю необходимо изменить логику вычисления некоторых встроенных функций, это свойство следует установить в true. В противном случае оставьте его в false с точки зрения производительности.

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


Указывает, требуется ли этому движку вычислять параметр в режиме массива. Значение по умолчанию — false. Если при вычислении пользовательских функций требуется [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) и пользователь не обновил их определение (с помощью [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-)), это свойство следует установить в true.

**Remarks**

Если этому пользовательскому движку вычислений требуется вычислять параметр в режиме массива, понадобится больше стеков для кэширования дерева параметров, и метод Calculate() может вызываться рекурсивно для вычисления значения параметра. С точки зрения производительности, пожалуйста, оставьте это свойство со значением по умолчанию (false), если нет особых требований.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Указывает, требуется ли этому движку буквальный текст параметра при выполнении расчёта. Значение по умолчанию — false.

**Remarks**

Если этому пользовательскому движку расчётов требуется буквальный текст параметра, понадобится больше стеков для кэширования буквального текста параметров, и метод Calculate() может вызываться рекурсивно для вычисления значения параметра. Как правило, буквальный текст не нужен при расчёте формул, и это свойство следует оставлять false для большинства реализаций, чтобы обеспечить лучшую производительность.

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


Пропускает вычисление всей формулы, которая ссылается на функцию, находящуюся в текущей оценке.

**Remarks**

Этот метод может быть вызван в реализации [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) для пропуска вычисления всей формулы, и исходное значение формулы будет сохранено без изменений.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

