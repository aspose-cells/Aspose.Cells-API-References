---
title: "Валидация"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет data validation.settings."
type: docs
url: /ru/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

Представляет data validation.settings.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Применяет проверку к области. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Применяет проверку к области. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Применяет проверку к указанным областям. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Копировать проверку. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Представляет стиль оповещения проверки. |
| [getAreas()](#getAreas--) | Получает все [CellArea](../../com.aspose.cells/cellarea), содержащие настройки проверки данных. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Представляет сообщение об ошибке проверки данных. |
| [getErrorTitle()](#getErrorTitle--) | Представляет заголовок диалогового окна ошибки проверки данных. |
| [getFormula1()](#getFormula1--) | Представляет значение или выражение, связанное с проверкой данных. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Получает значение или выражение, связанное с этой проверкой. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [getFormula2()](#getFormula2--) | Представляет значение или выражение, связанное с проверкой данных. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Получает значение или выражение, связанное с этой проверкой. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Указывает, допускаются ли пустые значения в проверке диапазона данных. |
| [getInCellDropDown()](#getInCellDropDown--) | Указывает, отображает ли проверка данных выпадающий список, содержащий допустимые значения. |
| [getInputMessage()](#getInputMessage--) | Представляет сообщение ввода проверки данных. |
| [getInputTitle()](#getInputTitle--) | Представляет заголовок диалогового окна ввода проверки данных. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Получить значение списка проверки для указанной ячейки. |
| [getOperator()](#getOperator--) | Представляет оператор проверки данных. |
| [getShowError()](#getShowError--) | Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные. |
| [getShowInput()](#getShowInput--) | Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [getType()](#getType--) | Представляет тип проверки данных. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Получить значение проверки в конкретной ячейке. |
| [getValue1()](#getValue1--) | Представляет первое значение, связанное с проверкой данных. |
| [getValue2()](#getValue2--) | Представляет второе значение, связанное с проверкой данных. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Удалить настройки проверки в ячейке. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Удалить настройки проверки в диапазоне. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Удаляет эту проверку из указанных областей. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Представляет стиль оповещения проверки. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Представляет сообщение об ошибке проверки данных. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Представляет заголовок диалогового окна ошибки проверки данных. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Представляет значение или выражение, связанное с проверкой данных. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Устанавливает значение или выражение, связанное с этой проверкой. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Представляет значение или выражение, связанное с проверкой данных. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Устанавливает значение или выражение, связанное с этой проверкой. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Указывает, допускаются ли пустые значения в проверке диапазона данных. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Указывает, отображает ли проверка данных выпадающий список, содержащий допустимые значения. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Представляет сообщение ввода проверки данных. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Представляет заголовок диалогового окна ввода проверки данных. |
| [setOperator(int value)](#setOperator-int-) | Представляет оператор проверки данных. |
| [setShowError(boolean value)](#setShowError-boolean-) | Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [setType(int value)](#setType-int-) | Представляет тип проверки данных. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Представляет первое значение, связанное с проверкой данных. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Представляет второе значение, связанное с проверкой данных. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


Применяет проверку к области.

**Remarks**

Это эквивалентно использованию [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) с проверкой пересечения и границы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Область. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


Применяет проверку к области.

**Remarks**

В этом методе мы удалим все старые проверки в указанной области. Для верхней‑левой области применённых диапазонов проверки сначала её StartRow минимален, затем её StartColumn минимален среди областей с тем же минимальным StartRow.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Область. |
| checkIntersection | boolean | Определяет, проверять ли пересечение заданной области с областями существующих проверок. Если в заданной области (или её части) уже применена проверка, то существующая проверка должна сначала быть удалена из этой области. В противном случае может возникнуть повреждение сгенерированных проверок. Если пользователь уверен, что добавляемая область не пересекается ни с одной существующей областью, этот параметр можно установить в false для повышения производительности. |
| checkEdge | boolean | Определяет, проверять ли границу применённых областей этой проверки. Внутренние настройки проверки зависят от верхней‑левой области её применённых диапазонов, поэтому если заданная область станет новой верхней‑левой областью применённых диапазонов, внутренние настройки должны быть изменены и перестроены, иначе может возникнуть неожиданный результат. Если пользователь уверен, что добавляемая область не является верхней‑левой, этот параметр можно установить в false для повышения производительности. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


Применяет проверку к указанным областям.

**Remarks**

В этом методе мы удалим все старые проверки в указанной области. Для верхней‑левой области применённых диапазонов проверки сначала её StartRow минимален, затем её StartColumn минимален среди областей с тем же минимальным StartRow.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Области. |
| checkIntersection | boolean | Определяет, проверять ли пересечение заданной области с областями существующих проверок. Если в заданной области (или её части) уже применена проверка, то существующая проверка должна сначала быть удалена из этой области. В противном случае может возникнуть повреждение сгенерированных проверок. Если пользователь уверен, что все добавляемые области не пересекаются ни с одной существующей областью, этот параметр можно установить в false для повышения производительности. |
| checkEdge | boolean | Определяет, проверять ли границу применённых областей этой проверки. Внутренние настройки проверки зависят от верхней‑левой области её применённых диапазонов, поэтому если одна из заданных областей станет новой верхней‑левой областью применённых диапазонов, внутренние настройки должны быть изменены и перестроены, иначе может возникнуть неожиданный результат. Если пользователь уверен, что ни одна из добавляемых областей не является верхней‑левой, этот параметр можно установить в false для повышения производительности. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


Копировать проверку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | Исходная проверка. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | Опция копирования. |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


Представляет стиль оповещения проверки.

Смотрите [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Получает все [CellArea](../../com.aspose.cells/cellarea), содержащие настройки проверки данных.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


Представляет сообщение об ошибке проверки данных.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Представляет заголовок диалогового окна ошибки проверки данных.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Представляет значение или выражение, связанное с проверкой данных.

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Получает значение или выражение, связанное с этой проверкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String - Значение или выражение, связанное с этой проверкой.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Получает значение или выражение, связанное с этой проверкой для конкретной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String - Значение или выражение, связанное с этой проверкой.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Представляет значение или выражение, связанное с проверкой данных.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Получает значение или выражение, связанное с этой проверкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String - Значение или выражение, связанное с этой проверкой.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Получает значение или выражение, связанное с этой проверкой для конкретной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String - Значение или выражение, связанное с этой проверкой.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


Указывает, допускаются ли пустые значения в проверке диапазона данных.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


Указывает, отображает ли проверка данных выпадающий список, содержащий допустимые значения.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Представляет сообщение ввода проверки данных.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Представляет заголовок диалогового окна ввода проверки данных.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Получить значение списка проверки для указанной ячейки.

**Remarks**

Только для проверки, тип которой List, и которая применена к указанной ячейке; в противном случае будет возвращено null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.Object - Значение для формирования списка этой проверки для указанной ячейки. Если список ссылается на диапазон, то возвращаемое значение будет объектом [ReferredArea](../../com.aspose.cells/referredarea); в противном случае возвращаемое значение может быть null, object[] или простым объектом.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Представляет оператор проверки данных.

Смотрите [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Представляет тип проверки данных.

Смотрите [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


Получить значение проверки в конкретной ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |
| isValue1 | boolean | Указывает, получено ли первое значение. |

**Returns:**
java.lang.Object - 
### getValue1() {#getValue1--}
```
public Object getValue1()
```


Представляет первое значение, связанное с проверкой данных.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


Представляет второе значение, связанное с проверкой данных.

**Returns:**
java.lang.Object
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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Удалить настройки проверки в ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


Удалить настройки проверки в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Области, в которых следует удалить эти настройки проверки. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


Удаляет эту проверку из указанных областей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Области, в которых следует удалить эти настройки проверки. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


Представляет стиль оповещения проверки.

Смотрите [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Представляет сообщение об ошибке проверки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Представляет заголовок диалогового окна ошибки проверки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Представляет значение или выражение, связанное с проверкой данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Устанавливает значение или выражение, связанное с этой проверкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Значение или выражение, связанное с этим условием форматирования. |
| isR1C1 | boolean | Является ли формула формулой R1C1. |
| isLocal | boolean | Отформатирована ли формула в соответствии с локалью. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Представляет значение или выражение, связанное с проверкой данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Устанавливает значение или выражение, связанное с этой проверкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Значение или выражение, связанное с этим условием форматирования. |
| isR1C1 | boolean | Является ли формула формулой R1C1. |
| isLocal | boolean | Отформатирована ли формула в соответствии с локалью. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


Указывает, допускаются ли пустые значения в проверке диапазона данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


Указывает, отображает ли проверка данных выпадающий список, содержащий допустимые значения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Представляет сообщение ввода проверки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Представляет заголовок диалогового окна ввода проверки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Представляет оператор проверки данных.

Смотрите [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Представляет тип проверки данных.

Смотрите [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


Представляет первое значение, связанное с проверкой данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


Представляет второе значение, связанное с проверкой данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

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

