---
title: PageCount
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ottiene o imposta il numero di pagine da salvare.
type: docs
weight: 240
url: /it/net/aspose.cells/pdfsaveoptions/pagecount/
---
## PdfSaveOptions.PageCount property

Ottiene o imposta il numero di pagine da salvare.

```csharp
public int PageCount { get; set; }
```

### Osservazioni

L'impostazione predefinita è System.Int32.MaxValue, il che significa che tutte le pagine verranno visualizzate..

### Esempi

L'esempio seguente mostra come eseguire il rendering di un intervallo di pagine (3 e 4) in un file Microsoft Excel in PDF.

```csharp
//Apri un file Excel
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions options = new PdfSaveOptions();

//Stampa solo pagina 3 e pagina 4 nel PDF di output
//Indice pagina iniziale (indice basato su 0)
options.PageIndex = 3;
//Numero di pagine da stampare
options.PageCount = 2;

//Salva il file PDF
wb.Save("output.pdf", options);
```

### Guarda anche

* class [PdfSaveOptions](../../pdfsaveoptions)
* spazio dei nomi [Aspose.Cells](../../pdfsaveoptions)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
