---
title: BorderWeight
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ottiene o imposta lo spessore della linea di confine di unimmagine in unità di pt.
type: docs
weight: 20
url: /it/net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Ottiene o imposta lo spessore della linea di confine di un'immagine in unità di pt.

```csharp
public double BorderWeight { get; set; }
```

### Esempi

```csharp

[C#]
//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//Aggiunta di un'immagine nella posizione di una cella i cui indici di riga e colonna sono 1 nel foglio di lavoro. È la cella "B2".
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
//Ottieni l'oggetto immagine inserito
Picture pic = worksheet.Pictures[imgIndex];
//Imposta il colore del bordo dell'immagine
pic.BorderLineColor = Color.Red;
//Imposta la larghezza del bordo dell'immagine
pic.BorderWeight = 3;
//Salva il file excel.
workbook.Save("result.xlsx");
```

### Guarda anche

* class [Picture](../../picture)
* spazio dei nomi [Aspose.Cells.Drawing](../../picture)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->