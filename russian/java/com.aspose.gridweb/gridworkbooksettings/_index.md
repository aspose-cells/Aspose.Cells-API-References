---
title: "GridWorkbookSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройки рабочей книги."
type: docs
url: /ru/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

Представляет настройки рабочей книги.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | конструктор по умолчанию |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Получает автора файла. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Определяет, проверяется ли пользовательский числовой формат при установке Style.Custom. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Определяет, создаётся ли цепочка вычисляемых формул. |
| [getDate1904()](#getDate1904--) | Получает значение, указывающее, использует ли рабочая книга систему дат 1904 года. |
| [getEnableMacros()](#getEnableMacros--) | Определяет, включены ли макросы; сейчас это работает только при копировании листа в другой лист в рабочей книге. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Получает, полностью ли вычисляется каждый раз при запуске расчёта. |
| [getIteration()](#getIteration--) | Получает, используется ли итерация для разрешения циклических ссылок. |
| [getMaxIteration()](#getMaxIteration--) | Получает максимальное количество итераций для разрешения циклической ссылки, значение по умолчанию — 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | True, если расчёты в этой рабочей книге будут выполнены только с точностью чисел, как они отображаются |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Получает, следует ли пересчитывать все формулы при открытии файла. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Устанавливает автора файла. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Устанавливает, проверять ли пользовательский числовой формат при установке Style.Custom. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Устанавливает, создавать ли цепочку вычисляемых формул. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Устанавливает значение, указывающее, использует ли рабочая книга систему дат 1904 года. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Устанавливает, включать ли макросы; сейчас это работает только при копировании листа в другой лист в рабочей книге. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Устанавливает, полностью ли вычислять каждый раз при запуске расчёта. |
| [setIteration(boolean value)](#setIteration-boolean-) | Устанавливает, использовать ли итерацию для разрешения циклических ссылок. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Устанавливает максимальное количество итераций для разрешения циклической ссылки, значение по умолчанию — 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | True, если расчёты в этой рабочей книге будут выполнены только с точностью чисел, как они отображаются |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Устанавливает, пересчитывать ли все формулы при открытии файла. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


конструктор по умолчанию

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Получает автора файла.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Определяет, проверяется ли пользовательский числовой формат при установке Style.Custom.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Получает, создавать ли цепочку вычисляемых формул. По умолчанию — false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Получает значение, указывающее, использует ли рабочая книга систему дат 1904 года.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Определяет, включены ли макросы; сейчас это работает только при копировании листа в другой лист в рабочей книге.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Получает, полностью ли вычисляется каждый раз при запуске расчёта.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Получает, используется ли итерация для разрешения циклических ссылок.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Получает максимальное количество итераций для разрешения циклической ссылки, значение по умолчанию — 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


True, если расчёты в этой рабочей книге будут выполнены только с точностью чисел, как они отображаются

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

Обычно эти пробелы и разрывы строк нужны только для визуального оформления; их сохранение или отсутствие не влияет на вычисленный результат. В целях производительности, если нет особых требований, лучше не сохранять их при обработке формул.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Получает, следует ли пересчитывать все формулы при открытии файла.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Устанавливает автора файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Устанавливает, проверять ли пользовательский числовой формат при установке Style.Custom.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Устанавливает, создавать ли цепочку вычисляемых формул. По умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Устанавливает значение, указывающее, использует ли рабочая книга систему дат 1904 года.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Устанавливает, включать ли макросы; сейчас это работает только при копировании листа в другой лист в рабочей книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Устанавливает, полностью ли вычислять каждый раз при запуске расчёта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Устанавливает, использовать ли итерацию для разрешения циклических ссылок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Устанавливает максимальное количество итераций для разрешения циклической ссылки, значение по умолчанию — 100.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


True, если расчёты в этой рабочей книге будут выполнены только с точностью чисел, как они отображаются

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

Обычно эти пробелы и разрывы строк нужны только для визуального оформления; их сохранение или отсутствие не влияет на вычисленный результат. В целях производительности, если нет особых требований, лучше не сохранять их при обработке формул.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Устанавливает, пересчитывать ли все формулы при открытии файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

