---
title: "GridValidationType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет тип проверки данных."
type: docs
url: /ru/java/com.aspose.gridweb/gridvalidationtype/
---

**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```

Представляет тип проверки данных.
## Поля

| Поле | Описание |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | Тип проверки любого значения. |
| [BOOLEAN](#BOOLEAN) | TRUE или FALSE |
| [CHECK_BOX](#CHECK-BOX) | Отобразить ячейку как флажок. |
| [CUSTOM](#CUSTOM) | Пользовательский тип проверки. |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | Пользовательский тип проверки, использующий регулярное выражение. |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | Пользовательская проверка функцией JavaScript. |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | Пользовательская проверка серверной функции. |
| [DATE](#DATE) | Тип проверки даты. |
| [DATE_TIME](#DATE-TIME) | Дата и время (yyyy-MM-dd или yyyy-MM-dd hh:mm:ss). |
| [DECIMAL](#DECIMAL) | Тип проверки десятичного числа. |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | Показать выпадающий список. |
| [FREE_LIST](#FREE-LIST) | Тип проверки свободного списка. |
| [LIST](#LIST) | Тип проверки списка. |
| [TEXT_LENGTH](#TEXT-LENGTH) | Тип проверки длины текста. |
| [TIME](#TIME) | Тип проверки времени. |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | Тип проверки целого числа. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ANY_VALUE {#ANY-VALUE}
```
public static final int ANY_VALUE
```


Тип проверки любого значения.

### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```


TRUE или FALSE

### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```


Отобразить ячейку как флажок. И значение ячейки — True или False.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Пользовательский тип проверки.

### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```


Пользовательский тип проверки, использующий регулярное выражение.

### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```


Пользовательская проверка функцией JavaScript.

**Remarks**

Используйте свойство ClientValidationFunction, чтобы указать имя функции клиентской проверки. Функция должна быть объявлена в следующем виде:
function customValicationFunction(source, value)
Параметр \"source\" — объект ячейки. Параметр \"value\" — строковое значение ячейки, которое нужно проверить. Функция должна возвращать true, если значение корректно.

### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```


Пользовательская проверка серверной функции.

**Remarks**

Используйте свойство CustomServerFunction, чтобы указать серверную проверку. Ниже приведён пример кода:
Сначала определите класс, реализующий GridCustomServerValidation: class myservervali : GridCustomServerValidation
...... затем добавьте проверку var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); затем установите ClientValidationFunction, чтобы обработать клиентскую логику при ошибке серверной проверки и вернуть сообщение gv.ClientValidationFunction = \"ValidationErrorClientFunction\"; клиентская функция должна быть объявлена следующим образом: function ValidationErrorClientFunction(cell,msg) пожалуйста, проверьте демонстрационную страницу для подробного справочного материала

### DATE {#DATE}
```
public static final int DATE
```


Тип проверки даты.

### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```


Дата и время (yyyy-MM-dd или yyyy-MM-dd hh:mm:ss).

### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Тип проверки десятичного числа.

### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```


Показать выпадающий список.

### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```


Тип проверки свободного списка.

### LIST {#LIST}
```
public static final int LIST
```


Тип проверки списка.

### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```


Тип проверки длины текста.

### TIME {#TIME}
```
public static final int TIME
```


Тип проверки времени.

### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```


Тип проверки целого числа.

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

