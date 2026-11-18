---
title: "TextParagraph-klass"
linktitle: "TextParagraph"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "TextParagraph-klass. Inkapslar objektet som representerar textparagraph i Go."
type: docs
weight: 200
url: /sv/go-cpp/textparagraph/
---

## TextParagraph class

Representerar inställningen för textstycket.

```go

type TextParagraph struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewTextParagraph](./newtextparagraph/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetBullet](./getbullet/) | Hämtar punkttecknet. |
| [GetType](./gettype/) | Hämtar typen av textnod. |
| [GetLineSpaceSizeType](./getlinespacesizetype/) | Hämtar och anger mängden vertikalt blanksteg som kommer att användas inom ett stycke. |
| [SetLineSpaceSizeType](./setlinespacesizetype/) | Hämtar och anger mängden vertikalt blanksteg som kommer att användas inom ett stycke. |
| [GetLineSpace](./getlinespace/) | Hämtar och anger mängden vertikalt blanksteg som kommer att användas inom ett stycke. |
| [SetLineSpace](./setlinespace/) | Hämtar och anger mängden vertikalt blanksteg som kommer att användas inom ett stycke. |
| [GetSpaceAfterSizeType](./getspaceaftersizetype/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas efter ett stycke. |
| [SetSpaceAfterSizeType](./setspaceaftersizetype/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas efter ett stycke. |
| [GetSpaceAfter](./getspaceafter/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas efter ett stycke. |
| [SetSpaceAfter](./setspaceafter/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas efter ett stycke. |
| [GetSpaceBeforeSizeType](./getspacebeforesizetype/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas före ett stycke. |
| [SetSpaceBeforeSizeType](./setspacebeforesizetype/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas före ett stycke. |
| [GetSpaceBefore](./getspacebefore/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas före ett stycke. |
| [SetSpaceBefore](./setspacebefore/) | Hämtar och anger mängden vertikalt blanksteg som kommer att finnas före ett stycke. |
| [GetStops](./getstops/) | Hämtar tabbstopplista. |
| [IsLatinLineBreak](./islatinlinebreak/) | Anger om ett latinskt ord kan brytas på mitten och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [SetIsLatinLineBreak](./setislatinlinebreak/) | Anger om ett latinskt ord kan brytas på mitten och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [IsEastAsianLineBreak](./iseastasianlinebreak/) | Anger om ett östasiatiskt ord kan brytas på mitten och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [SetIsEastAsianLineBreak](./setiseastasianlinebreak/) | Anger om ett östasiatiskt ord kan brytas på mitten och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [IsHangingPunctuation](./ishangingpunctuation/) | Anger om interpunktion ska tvingas placeras på en textrad eller placeras på en annan textrad. |
| [SetIsHangingPunctuation](./setishangingpunctuation/) | Anger om interpunktion ska tvingas placeras på en textrad eller placeras på en annan textrad. |
| [GetRightMargin](./getrightmargin/) | Anger högermarginalen för stycket. |
| [SetRightMargin](./setrightmargin/) | Anger högermarginalen för stycket. |
| [GetLeftMargin](./getleftmargin/) | Anger vänstermarginalen för stycket. |
| [SetLeftMargin](./setleftmargin/) | Anger vänstermarginalen för stycket. |
| [GetFirstLineIndent](./getfirstlineindent/) | Anger indenteringsstorleken som ska tillämpas på den första textraden i stycket. |
| [SetFirstLineIndent](./setfirstlineindent/) | Anger indenteringsstorleken som ska tillämpas på den första textraden i stycket. |
| [GetFontAlignType](./getfontaligntype/) | Bestämmer var vertikalt på en textrad de faktiska orden placeras. Detta handlar om vertikal placering av tecknen i förhållande till baslinjerna. |
| [SetFontAlignType](./setfontaligntype/) | Bestämmer var vertikalt på en textrad de faktiska orden placeras. Detta handlar om vertikal placering av tecknen i förhållande till baslinjerna. |
| [GetAlignmentType](./getalignmenttype/) | Hämtar och anger den horisontella justeringstypen för text i stycket. |
| [SetAlignmentType](./setalignmenttype/) | Hämtar och anger den horisontella justeringstypen för text i stycket. |
| [GetDefaultTabSize](./getdefaulttabsize/) | Hämtar och anger standardstorleken för ett tabulatortecken inom detta stycke. |
| [SetDefaultTabSize](./setdefaulttabsize/) | Hämtar och anger standardstorleken för ett tabulatortecken inom detta stycke. |
| [GetChildren](./getchildren/) | Hämtar alla textrader i detta stycke. Om detta stycke är tomt, returnera själva stycket. |
| [GetStartIndex](./getstartindex/) | Hämtar startindexet för tecknen. |
| [GetLength](./getlength/) | Hämtar längden på tecknen. |
| [GetFont](./getfont/) | Returnerar teckensnittet för detta objekt. |
| [SetWordArtStyle](./setwordartstyle/) | Ställer in den förinställda WordArt-stilen. |
| [GetTextOptions](./gettextoptions/) | Returnerar textalternativen. |
