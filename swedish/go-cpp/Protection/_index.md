---
title: "Protection-klass"
linktitle: "Protection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Protection-klass. Inkapslar objektet som representerar protection i Go."
type: docs
weight: 200
url: /sv/go-cpp/protection/
---

## Protection class

Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett arbetsblad.

```go

type Protection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [Copy](./copy/) | Kopiera skyddsinformation. |
| [GetAllowDeletingColumn](./getallowdeletingcolumn/) | Anger om borttagning av kolumner är tillåten på ett skyddat kalkylblad. |
| [SetAllowDeletingColumn](./setallowdeletingcolumn/) | Anger om borttagning av kolumner är tillåten på ett skyddat kalkylblad. |
| [GetAllowDeletingRow](./getallowdeletingrow/) | Representerar om radernas borttagning är tillåten på ett skyddat kalkylblad. |
| [SetAllowDeletingRow](./setallowdeletingrow/) | Representerar om radernas borttagning är tillåten på ett skyddat kalkylblad. |
| [GetAllowFiltering](./getallowfiltering/) | Representerar om användaren får använda ett AutoFilter som skapades innan bladet skyddades. |
| [SetAllowFiltering](./setallowfiltering/) | Representerar om användaren får använda ett AutoFilter som skapades innan bladet skyddades. |
| [GetAllowFormattingCell](./getallowformattingcell/) | Representerar om formatering av celler är tillåten på ett skyddat kalkylblad. |
| [SetAllowFormattingCell](./setallowformattingcell/) | Representerar om formatering av celler är tillåten på ett skyddat kalkylblad. |
| [GetAllowFormattingColumn](./getallowformattingcolumn/) | Representerar om formatering av kolumner är tillåten på ett skyddat kalkylblad |
| [SetAllowFormattingColumn](./setallowformattingcolumn/) | Representerar om formatering av kolumner är tillåten på ett skyddat kalkylblad |
| [GetAllowFormattingRow](./getallowformattingrow/) | Representerar om formatering av rader är tillåten på ett skyddat kalkylblad |
| [SetAllowFormattingRow](./setallowformattingrow/) | Representerar om formatering av rader är tillåten på ett skyddat kalkylblad |
| [GetAllowInsertingColumn](./getallowinsertingcolumn/) | Representerar om infogning av kolumner är tillåten på ett skyddat kalkylblad |
| [SetAllowInsertingColumn](./setallowinsertingcolumn/) | Representerar om infogning av kolumner är tillåten på ett skyddat kalkylblad |
| [GetAllowInsertingHyperlink](./getallowinsertinghyperlink/) | Representerar om infogning av hyperlänkar är tillåten på ett skyddat kalkylblad |
| [SetAllowInsertingHyperlink](./setallowinsertinghyperlink/) | Representerar om infogning av hyperlänkar är tillåten på ett skyddat kalkylblad |
| [GetAllowInsertingRow](./getallowinsertingrow/) | Representerar om infogning av rader är tillåten på ett skyddat kalkylblad |
| [SetAllowInsertingRow](./setallowinsertingrow/) | Representerar om infogning av rader är tillåten på ett skyddat kalkylblad |
| [GetAllowSorting](./getallowsorting/) | Representerar om sorteringsalternativet är tillåtet på ett skyddat kalkylblad. |
| [SetAllowSorting](./setallowsorting/) | Representerar om sorteringsalternativet är tillåtet på ett skyddat kalkylblad. |
| [GetAllowUsingPivotTable](./getallowusingpivottable/) | Representerar om användaren får manipulera pivottabeller på ett skyddat kalkylblad. |
| [SetAllowUsingPivotTable](./setallowusingpivottable/) | Representerar om användaren får manipulera pivottabeller på ett skyddat kalkylblad. |
| [GetAllowEditingContent](./getalloweditingcontent/) | Representerar om användaren får redigera innehållet i låsta celler på ett skyddat kalkylblad. |
| [SetAllowEditingContent](./setalloweditingcontent/) | Representerar om användaren får redigera innehållet i låsta celler på ett skyddat kalkylblad. |
| [GetAllowEditingObject](./getalloweditingobject/) | Representerar om användaren får manipulera ritobjekt på ett skyddat kalkylblad. |
| [SetAllowEditingObject](./setalloweditingobject/) | Representerar om användaren får manipulera ritobjekt på ett skyddat kalkylblad. |
| [GetAllowEditingScenario](./getalloweditingscenario/) | Representerar om användaren får redigera scenarier på ett skyddat kalkylblad. |
| [SetAllowEditingScenario](./setalloweditingscenario/) | Representerar om användaren får redigera scenarier på ett skyddat kalkylblad. |
| [GetAllowSelectingLockedCell](./getallowselectinglockedcell/) | Representerar om användaren får markera låsta celler på ett skyddat kalkylblad. |
| [SetAllowSelectingLockedCell](./setallowselectinglockedcell/) | Representerar om användaren får markera låsta celler på ett skyddat kalkylblad. |
| [GetAllowSelectingUnlockedCell](./getallowselectingunlockedcell/) | Representerar om användaren får markera olåsta celler på ett skyddat kalkylblad. |
| [SetAllowSelectingUnlockedCell](./setallowselectingunlockedcell/) | Representerar om användaren får markera olåsta celler på ett skyddat kalkylblad. |
| [GetPassword](./getpassword/) | Representerar lösenordet för att skydda kalkylbladet. |
| [SetPassword](./setpassword/) | Representerar lösenordet för att skydda kalkylbladet. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Indikerar om kalkylbladet är skyddat med lösenord. |
| [VerifyPassword](./verifypassword/) | Verifierar lösenord. |
| [GetPasswordHash](./getpasswordhash/) | Hämtar hashvärdet för det aktuella lösenordet. |
