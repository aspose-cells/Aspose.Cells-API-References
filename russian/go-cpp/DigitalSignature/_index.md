---
title: "Класс DigitalSignature"
linktitle: "DigitalSignature"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс DigitalSignature. Инкапсулирует объект, представляющий цифровую подпись в Go."
type: docs
weight: 200
url: /ru/go-cpp/digitalsignature/
---

## DigitalSignature class

Подпись в файле.

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | Конструктор DigitalSignature. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | Конструктор DigitalSignature. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetComments](./getcomments/) | Назначение подписи. |
| [SetComments](./setcomments/) | Назначение подписи. |
| [GetSignTime](./getsigntime/) | Время, когда документ был подписан. |
| [SetSignTime](./setsigntime/) | Время, когда документ был подписан. |
| [GetId](./getid/) | Указывает GUID, который может быть сопоставлен с GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — пустой (все нули) GUID. |
| [SetId](./setid/) | Указывает GUID, который может быть сопоставлен с GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — пустой (все нули) GUID. |
| [GetText](./gettext/) | Указывает текст фактической подписи в цифровой подписи. Значение по умолчанию — пусто. |
| [SetText](./settext/) | Указывает текст фактической подписи в цифровой подписи. Значение по умолчанию — пусто. |
| [GetImage](./getimage/) | Указывает изображение для цифровой подписи. Значение по умолчанию — null. |
| [SetImage](./setimage/) | Указывает изображение для цифровой подписи. Значение по умолчанию — null. |
| [GetProviderId](./getproviderid/) | Указывает идентификатор класса поставщика подписи. Значение по умолчанию — пустой (все нули) GUID. |
| [SetProviderId](./setproviderid/) | Указывает идентификатор класса поставщика подписи. Значение по умолчанию — пустой (все нули) GUID. |
| [IsValid](./isvalid/) | Если эта цифровая подпись действительна и документ не был подделан, это значение будет истинным. |
| [GetXAdESType](./getxadestype/) | Тип XAdES. Значение по умолчанию — None (XAdES отключён). |
| [SetXAdESType](./setxadestype/) | Тип XAdES. Значение по умолчанию — None (XAdES отключён). |
