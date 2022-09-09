---
title: HtmlNote
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ottiene e imposta la stringa html che contiene i dati e alcuni formati in questo commento.
type: docs
weight: 90
url: /it/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Ottiene e imposta la stringa html che contiene i dati e alcuni formati in questo commento.

```csharp
public string HtmlNote { get; set; }
```

### Osservazioni

Se si tratta di un commento con thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarla come commento con thread.

### Esempi

```csharp

[C#]
comment1.HtmlNote = "<Font Style="FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;">This is a <b>test</b>.</Font>";
```

### Guarda anche

* class [Comment](../../comment)
* spazio dei nomi [Aspose.Cells](../../comment)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->