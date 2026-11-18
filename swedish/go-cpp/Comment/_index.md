---
title: "Comment klass"
linktitle: "Comment"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Kommentar-klass. Inkapslar objektet som representerar en kommentar i Go."
type: docs
weight: 200
url: /sv/go-cpp/comment/
---

## Comment class

Inkapslar objektet som representerar en cellkommentar.

```go

type Comment struct  {
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
| [GetAuthor](./getauthor/) | Hämtar och anger namn på den ursprungliga kommentarsförfattaren |
| [SetAuthor](./setauthor/) | Hämtar och anger namn på den ursprungliga kommentarsförfattaren |
| [GetCommentShape](./getcommentshape/) | Hämta ett Shape-objekt som representerar formen som är bifogad till den angivna kommentaren. |
| [GetRow](./getrow/) | Hämtar radindexet för kommentaren. |
| [GetColumn](./getcolumn/) | Hämtar kolumnindexet för kommentaren. |
| [IsThreadedComment](./isthreadedcomment/) | Anger om denna kommentar är en trådad kommentar. |
| [GetThreadedComments](./getthreadedcomments/) | Hämtar listan med trådade kommentarer; |
| [GetNote](./getnote/) | Representerar innehållet i kommentaren. |
| [SetNote](./setnote/) | Representerar innehållet i kommentaren. |
| [GetHtmlNote](./gethtmlnote/) | Hämtar och anger HTML-strängen som innehåller data och vissa format i denna kommentar. |
| [SetHtmlNote](./sethtmlnote/) | Hämtar och anger HTML-strängen som innehåller data och vissa format i denna kommentar. |
| [GetFont](./getfont/) | Hämtar teckensnittet för kommentaren. |
| [FormatCharacters](./formatcharacters/) | Formatera vissa tecken med teckensnittsinställningen. |
| [Characters](./characters/) | Returnerar ett Characters-objekt som representerar ett intervall av tecken inom kommentartexten. |
| [GetRichFormattings](./getrichformattings/) | Returnerar alla Characters-objekt som representerar ett intervall av tecken inom kommentartexten. |
| [IsVisible](./isvisible/) | Representerar om kommentaren är synlig eller inte. |
| [SetIsVisible](./setisvisible/) | Representerar om kommentaren är synlig eller inte. |
| [GetTextOrientationType](./gettextorientationtype/) | Hämtar och anger textorienteringstypen för kommentaren. |
| [SetTextOrientationType](./settextorientationtype/) | Hämtar och anger textorienteringstypen för kommentaren. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Hämtar och anger den horisontella justeringstypen för kommentaren. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Hämtar och anger den horisontella justeringstypen för kommentaren. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Hämtar och anger den vertikala justeringstypen för kommentaren. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Hämtar och anger den vertikala justeringstypen för kommentaren. |
| [GetAutoSize](./getautosize/) | Anger om storleken på kommentaren justeras automatiskt enligt dess innehåll. Obs: I vissa speciella fall (t.ex. Mac-miljö) kan denna inställning vara utan effekt. Om denna inställning inte har någon effekt, ersätt den med FitToTextSize(). |
| [SetAutoSize](./setautosize/) | Anger om storleken på kommentaren justeras automatiskt enligt dess innehåll. Obs: I vissa speciella fall (t.ex. Mac-miljö) kan denna inställning vara utan effekt. Om denna inställning inte har någon effekt, ersätt den med FitToTextSize(). |
| [GetHeightCM](./getheightcm/) | Representerar kommentariens höjd, i enheten centimeter. |
| [SetHeightCM](./setheightcm/) | Representerar kommentariens höjd, i enheten centimeter. |
| [GetWidthCM](./getwidthcm/) | Representerar kommentariens bredd, i enheten centimeter. |
| [SetWidthCM](./setwidthcm/) | Representerar kommentariens bredd, i enheten centimeter. |
| [GetWidth](./getwidth/) | Representerar kommentariens bredd, i enheten pixlar. |
| [SetWidth](./setwidth/) | Representerar kommentariens bredd, i enheten pixlar. |
| [GetHeight](./getheight/) | Representerar kommentariens höjd, i enheten pixlar. |
| [SetHeight](./setheight/) | Representerar kommentariens höjd, i enheten pixlar. |
| [GetWidthInch](./getwidthinch/) | Representerar kommentariens bredd, i enheten tum. |
| [SetWidthInch](./setwidthinch/) | Representerar kommentariens bredd, i enheten tum. |
| [GetHeightInch](./getheightinch/) | Representerar kommentariens höjd, i enheten tum. |
| [SetHeightInch](./setheightinch/) | Representerar kommentariens höjd, i enheten tum. |
