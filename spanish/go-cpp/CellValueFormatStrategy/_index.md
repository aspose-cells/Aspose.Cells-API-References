---
title: "Enumeración CellValueFormatStrategy"
linktitle: "CellValueFormatStrategy"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Enumeración CellValueFormatStrategy. Encapsula el objeto que representa cellvalueformatstrategy en Go."
type: docs
weight: 200
url: /es/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

Specifies how to apply style for the value of the cell.

```go

type CellValueFormatStrategy int32


```

## Fields

| Field | Description |
| --- | --- |
| [None](./none/) | Sin formato. |
| [CellStyle](./cellstyle/) | Solo formateado con el estilo original de la celda. |
| [DisplayStyle](./displaystyle/) | Formateado con el estilo mostrado de la celda. |
| [DisplayString](./displaystring/) | Obtiene la cadena mostrada en MS Excel.La principal diferencia con <see cref="DisplayStyle"/> es que esta opción también considera el efecto del ancho de columna.Si el ancho de columna es demasiado pequeño para mostrar la cadena formateada completamente,"#" puede mostrarse, al igual que lo hace MS Excel. |
