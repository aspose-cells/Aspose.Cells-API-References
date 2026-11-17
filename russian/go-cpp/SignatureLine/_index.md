---
title: "SignatureLine Класс"
linktitle: "SignatureLine"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "SignatureLine класс. Инкапсулирует объект, представляющий signatureline в Go."
type: docs
weight: 200
url: /ru/go-cpp/signatureline/
---

## SignatureLine class

Представляет строку подписи.

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetId](./getid/) | Получает или задает идентификатор этой строки подписи. |
| [SetId](./setid/) | Получает или задает идентификатор этой строки подписи. |
| [GetProviderId](./getproviderid/) | Получает или задает идентификатор поставщика подписи. |
| [SetProviderId](./setproviderid/) | Получает или задает идентификатор поставщика подписи. |
| [GetSigner](./getsigner/) | Получает или задает подписанта. |
| [SetSigner](./setsigner/) | Получает или задает подписанта. |
| [GetTitle](./gettitle/) | Получает или задает название исполнителя. |
| [SetTitle](./settitle/) | Получает или задает название исполнителя. |
| [GetEmail](./getemail/) | Получает или задает электронную почту исполнителя. |
| [SetEmail](./setemail/) | Получает или задает электронную почту исполнителя. |
| [IsLine](./isline/) | Указывает, является ли это строкой подписи. |
| [SetIsLine](./setisline/) | Указывает, является ли это строкой подписи. |
| [GetAllowComments](./getallowcomments/) | Указывает, могут ли быть прикреплены комментарии. |
| [SetAllowComments](./setallowcomments/) | Указывает, могут ли быть прикреплены комментарии. |
| [GetShowSignedDate](./getshowsigneddate/) | Указывает, показывать ли дату подписи. |
| [SetShowSignedDate](./setshowsigneddate/) | Указывает, показывать ли дату подписи. |
| [GetInstructions](./getinstructions/) | Получает или задает текст, отображаемый пользователю во время подписи. |
| [SetInstructions](./setinstructions/) | Получает или задает текст, отображаемый пользователю во время подписи. |
| [GetSignatureLineType](./getsignaturelinetype/) | Получает или задает тип подписи. Default - Когда установлено значение по умолчанию, соответствующее значение ProviderId фиксируется как {0000000000-0000-0000-0000-0000000000}. Stamp - Когда значение равно Stamp, соответствующее значение ProviderId обычно равно {000CD6A4-0000-0000-C000-000000000046}. Custom - Когда значение равно Custom, соответствующее значение ProviderId обычно должно быть задано пользователем. Оно должно быть получено из документации, поставляемой с провайдером. |
| [SetSignatureLineType](./setsignaturelinetype/) | Получает или задает тип подписи. Default - Когда установлено значение по умолчанию, соответствующее значение ProviderId фиксируется как {0000000000-0000-0000-0000-0000000000}. Stamp - Когда значение равно Stamp, соответствующее значение ProviderId обычно равно {000CD6A4-0000-0000-C000-000000000046}. Custom - Когда значение равно Custom, соответствующее значение ProviderId обычно должно быть задано пользователем. Оно должно быть получено из документации, поставляемой с провайдером. |
