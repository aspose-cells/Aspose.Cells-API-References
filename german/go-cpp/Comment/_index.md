---
title: "Comment Klasse"
linktitle: "Comment"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Comment-Klasse. Kapselt das Objekt, das einen Kommentar in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/comment/
---

## Comment class

Kapselt das Objekt, das einen Zellkommentar darstellt.

```go

type Comment struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetAuthor](./getauthor/) | Liest und setzt den Namen des ursprünglichen Kommentarautors |
| [SetAuthor](./setauthor/) | Liest und setzt den Namen des ursprünglichen Kommentarautors |
| [GetCommentShape](./getcommentshape/) | Liefert ein Shape-Objekt, das die an den angegebenen Kommentar angehängte Form darstellt. |
| [GetRow](./getrow/) | Liefert den Zeilenindex des Kommentars. |
| [GetColumn](./getcolumn/) | Liefert den Spaltenindex des Kommentars. |
| [IsThreadedComment](./isthreadedcomment/) | Gibt an, ob dieser Kommentar ein Threaded-Comment ist. |
| [GetThreadedComments](./getthreadedcomments/) | Liefert die Liste der Threaded-Comments; |
| [GetNote](./getnote/) | Stellt den Inhalt des Kommentars dar. |
| [SetNote](./setnote/) | Stellt den Inhalt des Kommentars dar. |
| [GetHtmlNote](./gethtmlnote/) | Liest und setzt die HTML-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält. |
| [SetHtmlNote](./sethtmlnote/) | Liest und setzt die HTML-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält. |
| [GetFont](./getfont/) | Liefert die Schriftart des Kommentars. |
| [FormatCharacters](./formatcharacters/) | Formatiert einige Zeichen mit der Schriftarteinstellung. |
| [Characters](./characters/) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Kommentartext darstellt. |
| [GetRichFormattings](./getrichformattings/) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Kommentartext darstellen. |
| [IsVisible](./isvisible/) | Stellt dar, ob der Kommentar sichtbar ist oder nicht. |
| [SetIsVisible](./setisvisible/) | Stellt dar, ob der Kommentar sichtbar ist oder nicht. |
| [GetTextOrientationType](./gettextorientationtype/) | Liest und setzt den Textorientierungstyp des Kommentars. |
| [SetTextOrientationType](./settextorientationtype/) | Liest und setzt den Textorientierungstyp des Kommentars. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Liest und setzt den horizontalen Ausrichtungstyp des Textes im Kommentar. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Liest und setzt den horizontalen Ausrichtungstyp des Textes im Kommentar. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Liest und setzt den vertikalen Ausrichtungstyp des Textes im Kommentar. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Liest und setzt den vertikalen Ausrichtungstyp des Textes im Kommentar. |
| [GetAutoSize](./getautosize/) | Gibt an, ob die Größe des Kommentars automatisch an den Inhalt angepasst wird. Hinweis: In einigen Sonderfällen (wie z.B. der Mac-Umgebung) kann diese Einstellung keine Wirkung zeigen. Wenn diese Einstellung keine Wirkung zeigt, ersetzen Sie sie bitte durch FitToTextSize(). |
| [SetAutoSize](./setautosize/) | Gibt an, ob die Größe des Kommentars automatisch an den Inhalt angepasst wird. Hinweis: In einigen Sonderfällen (wie z.B. der Mac-Umgebung) kann diese Einstellung keine Wirkung zeigen. Wenn diese Einstellung keine Wirkung zeigt, ersetzen Sie sie bitte durch FitToTextSize(). |
| [GetHeightCM](./getheightcm/) | Stellt die Höhe des Kommentars dar, in Zentimetern. |
| [SetHeightCM](./setheightcm/) | Stellt die Höhe des Kommentars dar, in Zentimetern. |
| [GetWidthCM](./getwidthcm/) | Stellt die Breite des Kommentars dar, in Zentimetern. |
| [SetWidthCM](./setwidthcm/) | Stellt die Breite des Kommentars dar, in Zentimetern. |
| [GetWidth](./getwidth/) | Stellt die Breite des Kommentars dar, in Pixeln. |
| [SetWidth](./setwidth/) | Stellt die Breite des Kommentars dar, in Pixeln. |
| [GetHeight](./getheight/) | Stellt die Höhe des Kommentars dar, in Pixeln. |
| [SetHeight](./setheight/) | Stellt die Höhe des Kommentars dar, in Pixeln. |
| [GetWidthInch](./getwidthinch/) | Stellt die Breite des Kommentars dar, in Zoll. |
| [SetWidthInch](./setwidthinch/) | Stellt die Breite des Kommentars dar, in Zoll. |
| [GetHeightInch](./getheightinch/) | Stellt die Höhe des Kommentars dar, in Zoll. |
| [SetHeightInch](./setheightinch/) | Stellt die Höhe des Kommentars dar, in Zoll. |
