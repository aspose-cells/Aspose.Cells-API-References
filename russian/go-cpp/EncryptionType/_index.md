---
title: "EncryptionType Enum"
linktitle: "EncryptionType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "EncryptionType enum. Инкапсулирует объект, представляющий encryptiontype в Go."
type: docs
weight: 200
url: /ru/go-cpp/encryptiontype/
---

## EncryptionType Enum

Тип шифрования. Используется только в excel2003. Мы будем шифровать рабочую книгу 2007/2010 с помощью SHA AES так же, как делает Excel, и этот EncryptionType будет игнорироваться.

```go

type EncryptionType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [XOR](./xor/) | Алгоритм шифрования XOR. |
| [Compatible](./compatible/) | Совместимо с Office 97/2000. |
| [EnhancedCryptographicProviderV1](./enhancedcryptographicproviderv1/) | Улучшенное шифрование. |
| [StrongCryptographicProvider](./strongcryptographicprovider/) | Алгоритм сильного шифрования. |
