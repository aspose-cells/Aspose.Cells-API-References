---
title: "MainWeb.SessionMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MainWeb‑property. Hämtar eller anger sessionsläget för rutnätet"
type: docs
url: /sv/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Hämtar eller anger sessionsläget för rutnätet.

```csharp
public SessionMode SessionMode { get; set; }
```

### Anmärkningar

Det finns 4 typer av sessionsläge: 1. Session (standard): Använd systemsession för att lagra bladdata. Vanligtvis använder asp.net InProc‑sessionsstatus. Rutnätet stödjer också \"StateServer\"‑utprocess‑sessionsstatus och SQLServer‑sessionsstatus. 2. ViewState: Använd sidans viewstate för att lagra bladdata. 3. Custom: Använd LoadCustomData‑ och SheetDataUpdated‑händelser för att lagra/återställa bladdata. 4. File: lagra/återställa bladdata i SessionStorePath. Detta är det föreslagna sättet och kan hålla filen permanent. När SessionMode.ViewState används kommer rutnätet att lagra vissa data i sidans viewstate. Detta minskar serverns minnesanvändning, men sidans storlek blir större och det påverkar den totala prestandan.

### Exempel

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### Se även

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


