---
title: "Enum SessionMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.SessionMode enum. Representerar sessionsläget för rutnätet"
type: docs
url: /sv/net/aspose.cells.gridweb/sessionmode/
---
## SessionMode enumeration

Representerar sessionsläget för rutnätet.

```csharp
public enum SessionMode
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Session | `0` | Använder systemsessionen för att lagra/återhämta rutnätets bladdata automatiskt. |
| ViewState | `1` | Använder sidans viewstate för att lagra/återhämta rutnätets bladdata automatiskt. |
| Custom | `2` | Använder LoadCustomData‑händelsen för att manuellt ladda rutnätets bladdata. Och använder SheetDataUpdated‑händelsen för att spara rutnätets bladdata. |
| File | `3` | Använder systemfilen för att lagra/återhämta rutnätets bladdata automatiskt, användaren måste ange SessionStorePath för att specificera filkatalogen. |

### Se även

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


