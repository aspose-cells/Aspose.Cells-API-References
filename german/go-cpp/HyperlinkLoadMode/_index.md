---
title: "HyperlinkLoadMode Aufzählung"
linktitle: "HyperlinkLoadMode"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "HyperlinkLoadMode Aufzählung. Kapselt das Objekt, das hyperlinkloadmode in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

Gibt an, wie Hyperlinks beim Laden von HTML behandelt werden.

```go

type HyperlinkLoadMode int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [Normal](./normal/) | Nur der erste Hyperlink in einer Zelle wird geladen, nachfolgende werden ignoriert. |
| [AllowMultiple](./allowmultiple/) | Alle Hyperlinks in einer Zelle werden zu <see cref=\"Worksheet.Hyperlinks\"/> hinzugefügt. Beachten Sie, dass MS Excel selbst nur einen Hyperlink pro Zelle unterstützt, sodass diese Option Dateien erzeugen kann, die Excel nicht vollständig rendern kann. |
