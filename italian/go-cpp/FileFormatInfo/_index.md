---
title: "Classe FileFormatInfo"
linktitle: "FileFormatInfo"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe FileFormatInfo. Incapsula l'oggetto che rappresenta fileformatinfo in Go."
type: docs
weight: 200
url: /it/go-cpp/fileformatinfo/
---

## FileFormatInfo class

Contiene i dati restituiti dai metodi di rilevamento del formato file di <see cref=\"FileFormatUtil\"/>.

```go

type FileFormatInfo struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewFileFormatInfo](./newfileformatinfo/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [IsProtectedByRMS](./isprotectedbyrms/) | Indica se il file è protetto da Microsoft Rights Management Server. |
| [IsEncrypted](./isencrypted/) | Restituisce true se il documento è crittografato e richiede una password per l'apertura. |
| [GetFileFormatType](./getfileformattype/) | Ottiene il formato file rilevato. |
| [GetLoadFormat](./getloadformat/) | Ottiene il formato di caricamento rilevato. |
