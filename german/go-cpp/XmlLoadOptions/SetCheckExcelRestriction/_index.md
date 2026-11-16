---
title: "SetCheckExcelRestriction‑Methode"
linktitle: "SetCheckExcelRestriction"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SetCheckExcelRestriction‑Methode. Kapselt die Funktion, die setcheckexcelrestriction in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/xmlloadoptions/setcheckexcelrestriction/
---

## SetCheckExcelRestriction function

Ob die Beschränkungen einer Excel‑Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K, etwa mit Cell.PutValue(string), eingeben, erhalten Sie bei true‑Eigenschaft eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabe‑Zeichenkettenwert als Zellwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen.

```go

func (instance *XmlLoadOptions) SetCheckExcelRestriction(value bool)  error

```

## Hinweise


## Siehe auch

* Class [XmlLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
