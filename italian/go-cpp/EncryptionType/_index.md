---
title: "EncryptionType Enum"
linktitle: "EncryptionType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "EncryptionType enum. Incapsula l'oggetto che rappresenta encryptiontype in Go."
type: docs
weight: 200
url: /it/go-cpp/encryptiontype/
---

## EncryptionType Enum

Tipo di crittografia. Solo utilizzato da excel2003. Cripteremo le cartelle di lavoro 2007/2010 usando SHA AES come fa Excel, e questo EncryptionType sarà ignorato.

```go

type EncryptionType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [XOR](./xor/) | Algoritmo di crittografia XOR. |
| [Compatible](./compatible/) | Compatibile con Office 97/2000. |
| [EnhancedCryptographicProviderV1](./enhancedcryptographicproviderv1/) | Crittografia avanzata. |
| [StrongCryptographicProvider](./strongcryptographicprovider/) | Algoritmo di crittografia forte. |
