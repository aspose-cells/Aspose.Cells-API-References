---
title: "Класс ProtectedRange"
linktitle: "ProtectedRange"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ProtectedRange. Инкапсулирует объект, представляющий protectedrange в Go."
type: docs
weight: 200
url: /ru/go-cpp/protectedrange/
---

## ProtectedRange class

Указанный диапазон, разрешённый для редактирования, когда защита листа включена.

```go

type ProtectedRange struct  {
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
| [GetName](./getname/) | Получает заголовок диапазона. Он используется как дескриптор, а не как определение именованного диапазона. |
| [SetName](./setname/) | Получает заголовок диапазона. Он используется как дескриптор, а не как определение именованного диапазона. |
| [GetCellArea](./getcellarea/) | Получает объект CellArea, представляющий область ячеек, которую нужно защитить. |
| [GetAreas](./getareas/) | Получает все упомянутые области. |
| [AddArea](./addarea/) | Добавляет упомянутую область к этому. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Указывает, защищён ли лист паролем. |
| [GetPassword](./getpassword/) | Представляет пароль для защиты диапазона. |
| [SetPassword](./setpassword/) | Представляет пароль для защиты диапазона. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | Дескриптор безопасности определяет учетные записи пользователей, которые могут редактировать этот диапазон без ввода пароля для доступа к диапазону. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | Дескриптор безопасности определяет учетные записи пользователей, которые могут редактировать этот диапазон без ввода пароля для доступа к диапазону. |
