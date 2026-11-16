---
title: "EncryptionType Enum"
linktitle: "EncryptionType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "EncryptionType enum. Encapsule l'objet qui représente encryptiontype en Go."
type: docs
weight: 200
url: /fr/go-cpp/encryptiontype/
---

## EncryptionType Enum

Type de chiffrement. Utilisé uniquement par excel2003. Nous chiffrerons le classeur 2007/2010 en utilisant SHA AES comme le fait Excel, et ce EncryptionType sera ignoré.

```go

type EncryptionType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [XOR](./xor/) | Algorithme de chiffrement XOR. |
| [Compatible](./compatible/) | Compatible Office 97/2000. |
| [EnhancedCryptographicProviderV1](./enhancedcryptographicproviderv1/) | Chiffrement amélioré. |
| [StrongCryptographicProvider](./strongcryptographicprovider/) | Algorithme de chiffrement fort. |
