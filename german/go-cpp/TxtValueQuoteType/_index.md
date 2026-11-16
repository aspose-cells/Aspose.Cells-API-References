---
title: "TxtValueQuoteType Aufzählung"
linktitle: "TxtValueQuoteType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "TxtValueQuoteType Aufzählung. Kapselt das Objekt, das txtvaluequotetype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/txtvaluequotetype/
---

## TxtValueQuoteType Enum

Gibt den Typ der Verwendung von Anführungszeichen für Werte in Textformatdateien an.

```go

type TxtValueQuoteType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [Normal](./normal/) | Alle Werte, die Sonderzeichen wie Anführungszeichen oder Trennzeichen enthalten, werden in Anführungszeichen gesetzt. Entspricht dem Verhalten von MS Excel beim Exportieren von Textdateien. |
| [Always](./always/) | Alle Werte werden immer in Anführungszeichen gesetzt. |
| [Minimum](./minimum/) | Nur Werte bei Bedarf in Anführungszeichen setzen. Zum Beispiel, wenn ein Wert ein Anführungszeichen enthält, das jedoch nicht am Anfang des Wertes steht, wird dieser Wert nicht in Anführungszeichen gesetzt. |
| [Never](./never/) | Alle Werte werden nicht in Anführungszeichen gesetzt. Die mit diesem Typ exportierte Textdatei kann möglicherweise nicht korrekt wieder eingelesen werden, weil die erforderlichen Anführungszeichen fehlen. |
