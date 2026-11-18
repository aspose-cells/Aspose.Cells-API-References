---
title: "Row-klass."
linktitle: "Row"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Radklass. Inkapslar objektet som representerar en rad i Go."
type: docs
weight: 200
url: /sv/go-cpp/row/
---

## Row class

Representerar en enskild rad i ett arbetsblad.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | Hämta cellen med ett specifikt index i cellsamlingen för denna rad. |
| [IsBlank](./isblank/) | Indikerar om raden innehåller någon data |
| [Get](./get/) | Hämtar cellen. |
| [GetEnumerator](./getenumerator/) | Hämtar cellernas enumerator |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Hämtar en enumerator som itererar celler genom denna rad. |
| [GetCellOrNull](./getcellornull/) | Hämtar cellen eller null på det specifika indexet. |
| [IsCollapsed](./iscollapsed/) | om raden är kollapsad |
| [SetIsCollapsed](./setiscollapsed/) | om raden är kollapsad |
| [GetHeight](./getheight/) | Hämtar och anger radens höjd i enheten punkter. |
| [SetHeight](./setheight/) | Hämtar och anger radens höjd i enheten punkter. |
| [IsHidden](./ishidden/) | Indikerar om raden är dold. |
| [SetIsHidden](./setishidden/) | Indikerar om raden är dold. |
| [GetIndex](./getindex/) | Hämtar indexet för denna rad. |
| [GetGroupLevel](./getgrouplevel/) | Hämtar gruppnivån för raden. |
| [SetGroupLevel](./setgrouplevel/) | Hämtar gruppnivån för raden. |
| [IsHeightMatched](./isheightmatched/) | Indikerar om radens höjd matchar den aktuella standardteckensnittinställningen i arbetsboken. Sant för denna egenskap betyder också att radens höjd är "automatisk" utan att ett anpassat höjdvärde har satts av användaren. |
| [SetIsHeightMatched](./setisheightmatched/) | Indikerar om radens höjd matchar den aktuella standardteckensnittinställningen i arbetsboken. Sant för denna egenskap betyder också att radens höjd är "automatisk" utan att ett anpassat höjdvärde har satts av användaren. |
| [GetStyle](./getstyle/) | Hämtar stil för denna rad. |
| [SetStyle](./setstyle/) | Anger stil för denna rad. |
| [GetHasCustomStyle](./gethascustomstyle/) | Indikerar om denna rad har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från arbetsboken). |
| [CopySettings](./copysettings/) | Kopiera radens inställningar, såsom stil, höjd, synlighet, ...etc. |
| [GetFirstCell](./getfirstcell/) | Hämtar det första cellobjektet i raden. |
| [GetFirstDataCell](./getfirstdatacell/) | Hämtar den första icke-tomma cellen i raden. |
| [GetLastCell](./getlastcell/) | Hämtar det sista cellobjektet i raden. |
| [GetLastDataCell](./getlastdatacell/) | Hämtar den sista icke-tomma cellen i raden. |
| [ApplyStyle](./applystyle/) | Tillämpar format för en hel rad. |
| [Equals_Object](./equals_object/) | Kontrollerar om detta objekt refererar till samma rad som ett annat. |
| [Equals_Row](./equals_row/) | Kontrollerar om detta objekt refererar till samma rad som ett annat radobjekt. |
