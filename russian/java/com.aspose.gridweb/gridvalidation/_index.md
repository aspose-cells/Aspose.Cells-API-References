---
title: "GridValidation"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет data validation.settings."
type: docs
url: /ru/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

Представляет data validation.settings.
## Поля

| Поле | Описание |
| --- | --- |
| [ServerValidation](#ServerValidation) | Получает или задает имя серверной функции JavaScript для проверки. |
## Методы

| Метод | Описание |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | добавьте параметры проверки в ячейку. |
| [addACell(String cellname)](#addACell-java.lang.String-) | добавьте параметры проверки в ячейку. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Применяет проверку к области. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Представляет коллекцию [GridCellArea](../../com.aspose.gridweb/gridcellarea), содержащую параметры проверки данных. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | Получает имя клиентской функции JavaScript для проверки. |
| [getErrorMessage()](#getErrorMessage--) | Представляет сообщение об ошибке проверки данных. |
| [getErrorTitle()](#getErrorTitle--) | Представляет заголовок диалогового окна ошибки проверки данных. |
| [getFormula1()](#getFormula1--) | Представляет значение или выражение, связанное с проверкой данных. |
| [getFormula2()](#getFormula2--) | Представляет значение или выражение, связанные со второй частью проверки данных. |
| [getInputMessage()](#getInputMessage--) | Представляет сообщение об ошибке проверки данных. |
| [getInputTitle()](#getInputTitle--) | Представляет заголовок диалогового окна ввода проверки данных. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Получить значение списка проверки для указанной ячейки. |
| [getOperator()](#getOperator--) | Представляет оператор проверки данных. |
| [getRegEx()](#getRegEx--) | Получает строку регулярного выражения. |
| [getShowError()](#getShowError--) | Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные. |
| [getShowInput()](#getShowInput--) | Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [getValidationType()](#getValidationType--) | Получает тип проверки. |
| [getValue1()](#getValue1--) | Представляет значение, связанное с проверкой данных. |
| [getValueList()](#getValueList--) | Получает объект списка значений. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Получает, требуется ли значение ячейки. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Удалить настройки проверки в ячейке. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Удалить настройки проверки в диапазоне. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | Задает имя клиентской функции JavaScript для проверки. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Представляет сообщение об ошибке проверки данных. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Представляет заголовок диалогового окна ошибки проверки данных. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Представляет значение или выражение, связанное с проверкой данных. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Представляет значение или выражение, связанные со второй частью проверки данных. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Представляет сообщение об ошибке проверки данных. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Представляет заголовок диалогового окна ввода проверки данных. |
| [setOperator(int value)](#setOperator-int-) | Представляет оператор проверки данных. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Задает строку регулярного выражения. |
| [setRequired(boolean value)](#setRequired-boolean-) | Задает, требуется ли значение ячейки. |
| [setShowError(boolean value)](#setShowError-boolean-) | Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [setValidationType(int value)](#setValidationType-int-) | Задает тип проверки. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Задает объект списка значений. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Получает или задает имя серверной функции JavaScript для проверки.

**Remarks**

Используйте свойство GridCustomServerValidation, чтобы указать серверную проверку.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


добавьте параметры проверки в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


добавьте параметры проверки в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellname | java.lang.String | имя ячейки. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


Применяет проверку к области.

**Remarks**

В этом методе мы удалим все старые проверки в этой области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Область. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


Представляет коллекцию [GridCellArea](../../com.aspose.gridweb/gridcellarea), содержащую параметры проверки данных.

**Remarks**

Старые проверки в области не будут удалены, если напрямую добавить их в этот список.

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


Получает имя клиентской функции JavaScript для проверки.

**Remarks**

Используйте свойство ClientValidationFunction, чтобы указать имя функции клиентской проверки. Функция должна быть объявлена в следующем виде:
function customValicationFunction(source, value)
Параметр \"source\" — объект ячейки. Параметр \"value\" — строковое значение ячейки, которое нужно проверить. Функция должна возвращать true, если значение корректно.

**Returns:**
java.lang.String
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
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Представляет значение или выражение, связанные со второй частью проверки данных.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Представляет сообщение об ошибке проверки данных.

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
java.lang.Object — Значение, которое генерирует список этой проверки для указанной ячейки. Если список ссылается на диапазон, то возвращаемое значение будет объектом ReferredArea; в противном случае возвращаемое значение может быть null, object[] или простым объектом.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Представляет оператор проверки данных.

Смотрите [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


Получает строку регулярного выражения.

**Returns:**
java.lang.String
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
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


Получает тип проверки.

Смотрите [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


Представляет значение, связанное с проверкой данных.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


Получает объект списка значений.

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


Получает, требуется ли значение ячейки.

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

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


Удалить настройки проверки в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Диапазон, содержащий настройки проверки данных. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


Задает имя клиентской функции JavaScript для проверки.

**Remarks**

Используйте свойство ClientValidationFunction, чтобы указать имя функции клиентской проверки. Функция должна быть объявлена в следующем виде:
function customValicationFunction(source, value)
Параметр \"source\" — объект ячейки. Параметр \"value\" — строковое значение ячейки, которое нужно проверить. Функция должна возвращать true, если значение корректно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Представляет значение или выражение, связанные со второй частью проверки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Представляет сообщение об ошибке проверки данных.

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

Смотрите [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


Задает строку регулярного выражения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


Задает, требуется ли значение ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


Задает тип проверки.

Смотрите [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


Задает объект списка значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.ArrayList<java.lang.String> |  |

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

