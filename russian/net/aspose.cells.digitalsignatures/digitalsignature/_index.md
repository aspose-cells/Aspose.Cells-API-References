---
title: DigitalSignature
second_title: Справочник по Aspose.Cells для .NET API
description: Подпись в файле.
type: docs
weight: 1390
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Подпись в файле.

```csharp
public class DigitalSignature
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DigitalSignature](digitalsignature#constructor_1)(X509Certificate2, string, DateTime) | Конструктор digitalSignature. Использует реализацию .Net. |
| [DigitalSignature](digitalsignature#constructor)(byte[], string, string, DateTime) | Конструктор digitalSignature. Использует реализацию Bouncy Castle. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate) { get; set; } | Объект сертификата, который использовался для подписи документа. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments) { get; set; } | Цель подписи. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id) { get; set; } | Указывает идентификатор GUID, который можно сопоставить с идентификатором GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — Пусто (все нули) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image) { get; set; } | Задает изображение для цифровой подписи. Значение по умолчанию равно null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid) { get; } | Если эта цифровая подпись действительна и документ не был подделан, это значение будет истинным. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid) { get; set; } | Указывает идентификатор класса поставщика подписи. Значение по умолчанию — Пусто (все нули) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime) { get; set; } | Время подписания документа. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text) { get; set; } | Задает текст фактической подписи в цифровой подписи. Значение по умолчанию — Пусто. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype) { get; set; } | Тип XAdES. Значение по умолчанию — None (XAdES отключен). |

### Смотрите также

* пространство имен [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->