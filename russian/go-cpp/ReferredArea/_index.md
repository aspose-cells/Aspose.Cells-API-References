---
title: "Класс ReferredArea"
linktitle: "ReferredArea"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ReferredArea. Инкапсулирует объект, представляющий referredarea в Go."
type: docs
weight: 200
url: /ru/go-cpp/referredarea/
---

## ReferredArea class

Представляет область, на которую ссылается формула.

```go

type ReferredArea struct  {
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
| [IsExternalLink](./isexternallink/) | Указывает, является ли это внешней ссылкой. |
| [GetExternalFileName](./getexternalfilename/) | Получить имя внешнего файла, если это внешняя ссылка. |
| [GetSheetName](./getsheetname/) | Указывает, на каком листе находится эта ссылка. |
| [GetSheetNames](./getsheetnames/) | Имена всех листов, на которые ссылается этот экземпляр. |
| [IsEntireRow](./isentirerow/) | Указывает, содержит ли эта область все столбцы (полную строку). |
| [IsEntireColumn](./isentirecolumn/) | Указывает, содержит ли эта область все строки (полный столбец). |
| [IsArea](./isarea/) | Указывает, является ли это областью. |
| [GetEndColumn](./getendcolumn/) | Конечный столбец области. |
| [GetStartColumn](./getstartcolumn/) | Начальный столбец области. |
| [GetEndRow](./getendrow/) | Конечная строка области. |
| [GetStartRow](./getstartrow/) | Начальная строка области. |
| [GetValues](./getvalues/) | Получает значения ячеек в этой области. |
| [GetValues_Bool](./getvalues_bool/) | Получает значения ячеек в этой области. |
| [GetValue_Int_Int](./getvalue_int_int/) | Получает значение ячейки с заданным смещением от верхнего левого угла этой области. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Получает значение ячейки с заданным смещением от верхнего левого угла этой области. |
| [ToString](./tostring/) | Возвращает ссылочный адрес этой области. Обычно это адрес ссылки, который может использоваться в формуле, например "Sheet1!A1:C3". |
