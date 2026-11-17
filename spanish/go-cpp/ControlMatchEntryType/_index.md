---
title: "ControlMatchEntryType Enum"
linktitle: "ControlMatchEntryType"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "ControlMatchEntryType enum. Encapsula el objeto que representa controlmatchentrytype en Go."
type: docs
weight: 200
url: /es/go-cpp/controlmatchentrytype/
---

## ControlMatchEntryType Enum

Represents how a ListBox or ComboBox searches its list as the user types.

```go

type ControlMatchEntryType int32


```

## Fields

| Field | Description |
| --- | --- |
| [FirstLetter](./firstletter/) | El control busca la siguiente entrada que comienza con el carácter ingresado.Repetidamente al escribir la misma letra se recorre todas las entradas que comienzan con esa letra. |
| [Complete](./complete/) | A medida que se escribe cada carácter, el control busca una entrada que coincida con todos los caracteres ingresados. |
| [None](./none/) | La lista no se buscará cuando se escriban caracteres. |
