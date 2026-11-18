---
title: "ReConnectionMethodType enum"
linktitle: "ReConnectionMethodType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ReConnectionMethodType enum. Inkapslar objektet som representerar reconnectionmethodtype i Go."
type: docs
weight: 200
url: /sv/go-cpp/reconnectionmethodtype/
---

## ReConnectionMethodType Enum

Anger vad kalkylbladsprogrammet ska göra när en anslutning misslyckas.

```go

type ReConnectionMethodType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Required](./required/) | Vid uppdatering, använd den befintliga anslutningsinformationen och om den visar sig vara ogiltig, hämta uppdaterad anslutningsinformation, om den finns tillgänglig från den externa anslutningsfilen. |
| [Always](./always/) | Vid varje uppdatering, hämta uppdaterad anslutningsinformation från den externa anslutningsfilen, om den är tillgänglig, och använd den istället för den befintliga anslutningsinformationen. I detta fall kommer datauppdateringen att misslyckas om den externa anslutningsfilen är otillgänglig. |
| [Never](./never/) | Hämta aldrig uppdaterad anslutningsinformation från den externa anslutningsfilen, även om den är tillgänglig och även om den befintliga anslutningsinformationen är ogiltig. |
