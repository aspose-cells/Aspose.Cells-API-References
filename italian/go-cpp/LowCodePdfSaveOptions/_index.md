---
title: "Classe LowCodePdfSaveOptions"
linktitle: "LowCodePdfSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe LowCodePdfSaveOptions. Incapsula l'oggetto che rappresenta lowcodepdfsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

Opzioni per salvare pdf in modo low code.

```go

type LowCodePdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | Costruttore predefinito. |
| [NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSaveFormat](./getsaveformat/) | Il formato di salvataggio per l'output. Per la conversione in pdf, può essere solo SaveFormat.Pdf. |
| [SetSaveFormat](./setsaveformat/) | Il formato di salvataggio per l'output. Per la conversione in pdf, può essere solo SaveFormat.Pdf. |
| [GetPdfOptions](./getpdfoptions/) | Le opzioni per salvare il file Pdf. |
| [SetPdfOptions](./setpdfoptions/) | Le opzioni per salvare il file Pdf. |
| [GetOutputFile](./getoutputfile/) | Ottiene e imposta il file (con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, OutputStream verrà ignorato. |
| [SetOutputFile](./setoutputfile/) | Ottiene e imposta il file (con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, OutputStream verrà ignorato. |
| [GetOutputStream](./getoutputstream/) | Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, OutputFile verrà ignorato. |
| [SetOutputStream](./setoutputstream/) | Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, OutputFile verrà ignorato. |
