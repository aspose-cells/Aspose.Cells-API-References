---
title: "LowCodeSaveOptions Classe"
linktitle: "LowCodeSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "LowCodeSaveOptions classe. Incapsula l'oggetto che rappresenta lowcodesaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

Opzioni per salvare i risultati generati in modo low code.

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetOutputFile](./getoutputfile/) | Ottiene e imposta il file (con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, OutputStream verrà ignorato. |
| [SetOutputFile](./setoutputfile/) | Ottiene e imposta il file (con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, OutputStream verrà ignorato. |
| [GetOutputStream](./getoutputstream/) | Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, OutputFile verrà ignorato. |
| [SetOutputStream](./setoutputstream/) | Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, OutputFile verrà ignorato. |
| [GetSaveFormat](./getsaveformat/) | Ottiene e imposta il formato di salvataggio per l'output. In generale, per processi specifici in modalità low code, sono consentiti solo alcuni formati specifici. Specificare il formato corretto per il processo corrispondente, altrimenti potrebbero verificarsi risultati inattesi o addirittura eccezioni. |
| [SetSaveFormat](./setsaveformat/) | Ottiene e imposta il formato di salvataggio per l'output. In generale, per processi specifici in modalità low code, sono consentiti solo alcuni formati specifici. Specificare il formato corretto per il processo corrispondente, altrimenti potrebbero verificarsi risultati inattesi o addirittura eccezioni. |
