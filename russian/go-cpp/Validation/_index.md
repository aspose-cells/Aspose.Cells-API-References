---
title: "Класс Validation"
linktitle: "Validation"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Validation. Инкапсулирует объект, представляющий validation в Go."
type: docs
weight: 200
url: /ru/go-cpp/validation/
---

## Validation class

Представляет параметры проверки данных.

```go

type Validation struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetOperator](./getoperator/) | Представляет оператор для проверки данных. |
| [SetOperator](./setoperator/) | Представляет оператор для проверки данных. |
| [GetAlertStyle](./getalertstyle/) | Представляет стиль оповещения проверки. |
| [SetAlertStyle](./setalertstyle/) | Представляет стиль оповещения проверки. |
| [GetType](./gettype/) | Представляет тип проверки данных. |
| [SetType](./settype/) | Представляет тип проверки данных. |
| [GetInputMessage](./getinputmessage/) | Представляет сообщение ввода проверки данных. |
| [SetInputMessage](./setinputmessage/) | Представляет сообщение ввода проверки данных. |
| [GetInputTitle](./getinputtitle/) | Представляет заголовок диалогового окна ввода проверки данных. |
| [SetInputTitle](./setinputtitle/) | Представляет заголовок диалогового окна ввода проверки данных. |
| [GetErrorMessage](./geterrormessage/) | Представляет сообщение об ошибке проверки данных. |
| [SetErrorMessage](./seterrormessage/) | Представляет сообщение об ошибке проверки данных. |
| [GetErrorTitle](./geterrortitle/) | Представляет заголовок диалогового окна ошибки проверки данных. |
| [SetErrorTitle](./seterrortitle/) | Представляет заголовок диалогового окна ошибки проверки данных. |
| [GetShowInput](./getshowinput/) | Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [SetShowInput](./setshowinput/) | Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [GetShowError](./getshowerror/) | Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные. |
| [SetShowError](./setshowerror/) | Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные. |
| [GetIgnoreBlank](./getignoreblank/) | Указывает, допускаются ли пустые значения в проверке диапазона данных. |
| [SetIgnoreBlank](./setignoreblank/) | Указывает, допускаются ли пустые значения в проверке диапазона данных. |
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Получает значение или выражение, связанное с этой проверкой. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Получает значение или выражение, связанное с этой проверкой. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Устанавливает значение или выражение, связанное с этой проверкой. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Устанавливает значение или выражение, связанное с этой проверкой. |
| [GetFormula1](./getformula1/) | Представляет значение или выражение, связанное с проверкой данных. |
| [SetFormula1_String](./setformula1_string/) | Представляет значение или выражение, связанное с проверкой данных. |
| [GetFormula2](./getformula2/) | Представляет значение или выражение, связанное с проверкой данных. |
| [SetFormula2_String](./setformula2_string/) | Представляет значение или выражение, связанное с проверкой данных. |
| [GetListValue](./getlistvalue/) | Получить значение списка проверки для указанной ячейки. |
| [GetValue1](./getvalue1/) | Представляет первое значение, связанное с проверкой данных. |
| [SetValue1](./setvalue1/) | Представляет первое значение, связанное с проверкой данных. |
| [GetValue2](./getvalue2/) | Представляет второе значение, связанное с проверкой данных. |
| [SetValue2](./setvalue2/) | Представляет второе значение, связанное с проверкой данных. |
| [GetValue](./getvalue/) | Получить значение проверки для конкретной ячейки. |
| [GetInCellDropDown](./getincelldropdown/) | Указывает, отображает ли проверка данных выпадающий список, содержащий допустимые значения. |
| [SetInCellDropDown](./setincelldropdown/) | Указывает, отображает ли проверка данных выпадающий список, содержащий допустимые значения. |
| [GetAreas](./getareas/) | Получает все CellArea, содержащие настройки проверки данных. |
| [AddArea_CellArea](./addarea_cellarea/) | Применяет проверку к области. |
| [AddArea_CellArea_Bool_Bool](./addarea_cellarea_bool_bool/) | Применяет проверку к области. |
| [AddAreas](./addareas/) | Применяет проверку к указанным областям. |
| [RemoveArea](./removearea/) | Удалить настройки проверки в диапазоне. |
| [RemoveAreas](./removeareas/) | Удаляет эту проверку из указанных областей. |
| [RemoveACell](./removeacell/) | Удалить настройки проверки в ячейке. |
| [Copy](./copy/) | Копировать проверку. |
