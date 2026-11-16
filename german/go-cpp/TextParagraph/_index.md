---
title: "TextParagraph Klasse"
linktitle: "TextParagraph"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "TextParagraph Klasse. Kapselt das Objekt, das den textparagraph in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/textparagraph/
---

## TextParagraph class

Stellt die Einstellung des Textabsatzes dar.

```go

type TextParagraph struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewTextParagraph](./newtextparagraph/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetBullet](./getbullet/) | Liefert das Aufzählungszeichen. |
| [GetType](./gettype/) | Liest den Typ des Textknotens. |
| [GetLineSpaceSizeType](./getlinespacesizetype/) | Liefert und setzt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [SetLineSpaceSizeType](./setlinespacesizetype/) | Liefert und setzt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [GetLineSpace](./getlinespace/) | Liefert und setzt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [SetLineSpace](./setlinespace/) | Liefert und setzt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [GetSpaceAfterSizeType](./getspaceaftersizetype/) | Liefert und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist. |
| [SetSpaceAfterSizeType](./setspaceaftersizetype/) | Liefert und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist. |
| [GetSpaceAfter](./getspaceafter/) | Liefert und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist. |
| [SetSpaceAfter](./setspaceafter/) | Liefert und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden ist. |
| [GetSpaceBeforeSizeType](./getspacebeforesizetype/) | Liefert und setzt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist. |
| [SetSpaceBeforeSizeType](./setspacebeforesizetype/) | Liefert und setzt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist. |
| [GetSpaceBefore](./getspacebefore/) | Liefert und setzt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist. |
| [SetSpaceBefore](./setspacebefore/) | Liefert und setzt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden ist. |
| [GetStops](./getstops/) | Liefert die Tabulatorstopp-Liste. |
| [IsLatinLineBreak](./islatinlinebreak/) | Gibt an, ob ein lateinisches Wort halbiert und in die nächste Zeile umgebrochen werden kann, ohne dass ein Bindestrich hinzugefügt wird. |
| [SetIsLatinLineBreak](./setislatinlinebreak/) | Gibt an, ob ein lateinisches Wort halbiert und in die nächste Zeile umgebrochen werden kann, ohne dass ein Bindestrich hinzugefügt wird. |
| [IsEastAsianLineBreak](./iseastasianlinebreak/) | Gibt an, ob ein ostasiatisches Wort halbiert und in die nächste Zeile umgebrochen werden kann, ohne dass ein Bindestrich hinzugefügt wird. |
| [SetIsEastAsianLineBreak](./setiseastasianlinebreak/) | Gibt an, ob ein ostasiatisches Wort halbiert und in die nächste Zeile umgebrochen werden kann, ohne dass ein Bindestrich hinzugefügt wird. |
| [IsHangingPunctuation](./ishangingpunctuation/) | Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen. |
| [SetIsHangingPunctuation](./setishangingpunctuation/) | Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen. |
| [GetRightMargin](./getrightmargin/) | Gibt den rechten Rand des Absatzes an. |
| [SetRightMargin](./setrightmargin/) | Gibt den rechten Rand des Absatzes an. |
| [GetLeftMargin](./getleftmargin/) | Gibt den linken Rand des Absatzes an. |
| [SetLeftMargin](./setleftmargin/) | Gibt den linken Rand des Absatzes an. |
| [GetFirstLineIndent](./getfirstlineindent/) | Gibt die Einzugsgröße an, die auf die erste Textzeile im Absatz angewendet wird. |
| [SetFirstLineIndent](./setfirstlineindent/) | Gibt die Einzugsgröße an, die auf die erste Textzeile im Absatz angewendet wird. |
| [GetFontAlignType](./getfontaligntype/) | Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert werden. Dies befasst sich mit der vertikalen Platzierung der Zeichen in Bezug auf die Grundlinien. |
| [SetFontAlignType](./setfontaligntype/) | Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert werden. Dies befasst sich mit der vertikalen Platzierung der Zeichen in Bezug auf die Grundlinien. |
| [GetAlignmentType](./getalignmenttype/) | Liefert und setzt den horizontalen Ausrichtungstyp des Textes im Absatz. |
| [SetAlignmentType](./setalignmenttype/) | Liefert und setzt den horizontalen Ausrichtungstyp des Textes im Absatz. |
| [GetDefaultTabSize](./getdefaulttabsize/) | Liefert und setzt die Standardgröße für ein Tabulatorzeichen innerhalb dieses Absatzes. |
| [SetDefaultTabSize](./setdefaulttabsize/) | Liefert und setzt die Standardgröße für ein Tabulatorzeichen innerhalb dieses Absatzes. |
| [GetChildren](./getchildren/) | Liefert alle Textabschnitte in diesem Absatz. Wenn dieser Absatz leer ist, wird der Absatz selbst zurückgegeben. |
| [GetStartIndex](./getstartindex/) | Ermittelt den Startindex der Zeichen. |
| [GetLength](./getlength/) | Ermittelt die Länge der Zeichen. |
| [GetFont](./getfont/) | Gibt die Schriftart dieses Objekts zurück. |
| [SetWordArtStyle](./setwordartstyle/) | Setzt den voreingestellten WordArt‑Stil. |
| [GetTextOptions](./gettextoptions/) | Gibt die Textoptionen zurück. |
