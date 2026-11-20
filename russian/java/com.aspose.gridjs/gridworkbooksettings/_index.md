---
title: "GridWorkbookSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройки рабочей книги."
type: docs
url: /ru/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Представляет настройки рабочей книги.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Получает автора файла. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Указывает, следует ли проверять пользовательский числовой формат при установке Style.Custom, значение по умолчанию — false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Указывает, следует ли создавать цепочку вычисляемых формул. |
| [getDate1904()](#getDate1904--) | Получает значение, которое показывает, использует ли рабочая книга систему дат 1904 года. |
| [getEnableMacros()](#getEnableMacros--) | Включить макросы; сейчас они работают только при копировании листа в другой лист в книге. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Указывает, выполнять ли полные вычисления каждый раз при срабатывании расчёта. |
| [getIteration()](#getIteration--) | Указывает, использовать ли итерацию для разрешения круговых ссылок. |
| [getMaxIteration()](#getMaxIteration--) | Возвращает или задает максимальное количество итераций для разрешения круговой ссылки, значение по умолчанию — 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | True, если расчёты в этой рабочей книге будут выполнены только с точностью чисел, как они отображаются |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Указывает, следует ли пересчитывать все формулы при открытии файла. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Устанавливает автора файла. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Указывает, следует ли проверять пользовательский числовой формат при установке Style.Custom, значение по умолчанию — false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Указывает, следует ли создавать цепочку вычисляемых формул. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Устанавливает значение, указывающее, использует ли книга систему дат 1904 года. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Включить макросы; сейчас они работают только при копировании листа в другой лист в книге. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Указывает, выполнять ли полные вычисления каждый раз при срабатывании расчёта. |
| [setIteration(boolean value)](#setIteration-boolean-) | Указывает, использовать ли итерацию для разрешения круговых ссылок. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Возвращает или задает максимальное количество итераций для разрешения круговой ссылки, значение по умолчанию — 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | True, если расчёты в этой рабочей книге будут выполнены только с точностью чисел, как они отображаются |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Указывает, следует ли пересчитывать все формулы при открытии файла. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


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


Указывает, следует ли проверять пользовательский числовой формат при установке Style.Custom, значение по умолчанию — false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Определяет, проверять ли ограничения файла Excel при изменении пользователем связанных с ячейками объектов. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, вы получите Exception. Если свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, позже не следует сохранять рабочую книгу в формате Excel. В противном случае может возникнуть неожиданная ошибка в сгенерированном файле Excel. Значение по умолчанию — false.

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


Указывает, создавать ли цепочку вычисляемых формул. Значение по умолчанию — false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Получает значение, которое показывает, использует ли рабочая книга систему дат 1904 года.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Включить макросы; сейчас они работают только при копировании листа в другой лист в книге.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Указывает, выполнять ли полные вычисления каждый раз при срабатывании расчёта.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Указывает, использовать ли итерацию для разрешения круговых ссылок.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Возвращает или задает максимальное количество итераций для разрешения круговой ссылки, значение по умолчанию — 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


True, если расчёты в этой рабочей книге будут выполнены только с точностью чисел, как они отображаются

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Указывает, пересчитывать ли все формулы при открытии файла. Значение по умолчанию — true.

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


Указывает, следует ли проверять пользовательский числовой формат при установке Style.Custom, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Определяет, проверять ли ограничения файла Excel при изменении пользователем связанных с ячейками объектов. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, вы получите Exception. Если свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, позже не следует сохранять рабочую книгу в формате Excel. В противном случае может возникнуть неожиданная ошибка в сгенерированном файле Excel. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Указывает, создавать ли цепочку вычисляемых формул. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Устанавливает значение, указывающее, использует ли книга систему дат 1904 года.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Включить макросы; сейчас они работают только при копировании листа в другой лист в книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Указывает, выполнять ли полные вычисления каждый раз при срабатывании расчёта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Указывает, использовать ли итерацию для разрешения круговых ссылок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Возвращает или задает максимальное количество итераций для разрешения круговой ссылки, значение по умолчанию — 100.

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

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Указывает, пересчитывать ли все формулы при открытии файла. Значение по умолчанию — true.

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

