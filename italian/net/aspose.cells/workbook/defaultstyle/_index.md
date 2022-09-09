---
title: DefaultStyle
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ottiene o imposta il valore predefinitoStyleaspose.cells/style oggetto della cartella di lavoro.
type: docs
weight: 130
url: /it/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Ottiene o imposta il valore predefinito[`Style`](../../style) oggetto della cartella di lavoro.

```csharp
public Style DefaultStyle { get; set; }
```

### Osservazioni

La proprietà DefaultStyle è utile per implementare uno stile per l'intera cartella di lavoro.

### Esempi

Il codice seguente crea e crea un'istanza di una nuova cartella di lavoro e imposta un valore predefinito[`Style`](../../style) ad esso.

```csharp
[C#]
Workbook workbook = new Workbook();
Style defaultStyle = workbook.DefaultStyle;
defaultStyle.Font.Name = "Tahoma";
workbook.DefaultStyle = defaultStyle;

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim defaultStyle as Style = workbook.DefaultStyle
defaultStyle.Font.Name = "Tahoma"
workbook.DefaultStyle = defaultStyle
```

### Guarda anche

* class [Style](../../style)
* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->