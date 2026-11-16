---
title: "ReConnectionMethodType Enum"
linktitle: "ReConnectionMethodType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ReConnectionMethodType Enum. Kapselt das Objekt, das den ReConnectionMethodType in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/reconnectionmethodtype/
---

## ReConnectionMethodType Enum

Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.

```go

type ReConnectionMethodType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [Required](./required/) | Bei einer Aktualisierung die vorhandenen Verbindungsinformationen verwenden und, falls sie ungültig werden, aktualisierte Verbindungsinformationen aus der externen Verbindungsdatei abrufen, falls verfügbar. |
| [Always](./always/) | Bei jeder Aktualisierung aktualisierte Verbindungsinformationen aus der externen Verbindungsdatei abrufen, falls verfügbar, und diese anstelle der vorhandenen Verbindungsinformationen verwenden. In diesem Fall schlägt die Datenaktualisierung fehl, wenn die externe Verbindungsdatei nicht verfügbar ist. |
| [Never](./never/) | Nie aktualisierte Verbindungsinformationen aus der externen Verbindungsdatei abrufen, selbst wenn sie verfügbar ist und selbst wenn die vorhandenen Verbindungsinformationen ungültig sind. |
