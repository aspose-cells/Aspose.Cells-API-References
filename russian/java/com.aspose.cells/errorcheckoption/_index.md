---
title: "ErrorCheckOption"
second_title: "Справочник API Aspose.Cells for Java"
description: "Настройка проверки ошибок, применяемая к определённым диапазонам."
type: docs
url: /ru/java/com.aspose.cells/errorcheckoption/
---

**Inheritance:**
java.lang.Object
```
public class ErrorCheckOption
```

Настройка проверки ошибок, применяемая к определённым диапазонам.

**Example**

```
           Workbook workbook = new Workbook();
           ErrorCheckOptionCollection opts = workbook.getWorksheets().get(0).getErrorCheckOptions();
           int optionIdx = opts.add();
           ErrorCheckOption opt = opts.get(optionIdx);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_FORMULA, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_RANGE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_DATE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_NUMBER, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.VALIDATION, false);
           opt.addRange(CellArea.createCellArea("A1", "B10"));
           workbook.save("Book1.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addRange(CellArea ca)](#addRange-com.aspose.cells.CellArea-) | Добавляет один затронутый диапазон этим параметром. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCountOfRange()](#getCountOfRange--) | Получает количество диапазонов, затронутых этим параметром. |
| [getRange(int index)](#getRange-int-) | Получает затронутый диапазон этого параметра по заданному индексу. |
| [hashCode()](#hashCode--) |  |
| [isErrorCheck(int errorCheckType)](#isErrorCheck-int-) | Проверяет, будет ли проверяться указанный тип ошибки. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeRange(int index)](#removeRange-int-) | Удаляет один диапазон по заданному индексу. |
| [setErrorCheck(int errorCheckType, boolean isCheck)](#setErrorCheck-int-boolean-) | Устанавливает, будет ли проверяться указанный тип ошибки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(CellArea ca) {#addRange-com.aspose.cells.CellArea-}
```
public int addRange(CellArea ca)
```


Добавляет один затронутый диапазон этим параметром.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | диапазон, который будет добавлен. |

**Returns:**
int — индекс добавленного диапазона в списке диапазонов этой настройки.
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfRange() {#getCountOfRange--}
```
public int getCountOfRange()
```


Получает количество диапазонов, затронутых этим параметром.

**Returns:**
int — количество диапазонов, влияющих на эту настройку.
### getRange(int index) {#getRange-int-}
```
public CellArea getRange(int index)
```


Получает затронутый диапазон этого параметра по заданному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс диапазона |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - return influenced range at given index.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isErrorCheck(int errorCheckType) {#isErrorCheck-int-}
```
public boolean isErrorCheck(int errorCheckType)
```


Проверяет, будет ли проверяться указанный тип ошибки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). тип ошибки может быть проверен |

**Returns:**
boolean — возвращает true, если указанный тип ошибки будет проверен (зеленый треугольник будет показан для ячейки, если проверка не удалась).
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeRange(int index) {#removeRange-int-}
```
public void removeRange(int index)
```


Удаляет один диапазон по заданному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс диапазона, который нужно удалить. |

### setErrorCheck(int errorCheckType, boolean isCheck) {#setErrorCheck-int-boolean-}
```
public void setErrorCheck(int errorCheckType, boolean isCheck)
```


Устанавливает, будет ли проверяться указанный тип ошибки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). тип ошибки может быть проверен. |
| isCheck | boolean | true, если указанный тип ошибки необходимо проверить (зеленый треугольник будет показан для ячейки, если проверка не удалась). |

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

