---
title: "SmartArtShape Klasse"
linktitle: "SmartArtShape"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SmartArtShape Klasse. Kapselt das Objekt, das smartartshape in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/smartartshape/
---

## SmartArtShape class

Stellt die SmartArt dar.

```go

type SmartArtShape struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewSmartArtShape](./newsmartartshape/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetResultOfSmartArt](./getresultofsmartart/) | Konvertiere SmartArt in gruppierte Formen. |
| [GetMacroName](./getmacroname/) | Liest und setzt den Namen des Makros. |
| [SetMacroName](./setmacroname/) | Liest und setzt den Namen des Makros. |
| [IsEquation](./isequation/) | Gibt an, ob die Form nur eine Gleichung enthält. |
| [IsSmartArt](./issmartart/) | Gibt an, ob die Form ein SmartArt ist. |
| [ToFrontOrBack](./tofrontorback/) | Bringt die Form nach vorne oder sendet die Form nach hinten. |
| [GetZOrderPosition](./getzorderposition/) | Gibt die Position einer Form in der Z‑Reihenfolge zurück. |
| [SetZOrderPosition](./setzorderposition/) | Gibt die Position einer Form in der Z‑Reihenfolge zurück. |
| [GetName](./getname/) | Liest und setzt den Namen der Form. |
| [SetName](./setname/) | Liest und setzt den Namen der Form. |
| [GetAlternativeText](./getalternativetext/) | Gibt den beschreibenden (alternativen) Textstring des Shape‑Objekts zurück oder setzt ihn. |
| [SetAlternativeText](./setalternativetext/) | Gibt den beschreibenden (alternativen) Textstring des Shape‑Objekts zurück oder setzt ihn. |
| [GetTitle](./gettitle/) | Legt den Titel (Beschriftung) des aktuellen Shape‑Objekts fest. |
| [SetTitle](./settitle/) | Legt den Titel (Beschriftung) des aktuellen Shape‑Objekts fest. |
| [GetLine](./getline/) | Liest den Linienstil |
| [GetFill](./getfill/) | Gibt ein FillFormat‑Objekt zurück, das Füllformatierungseigenschaften für die angegebene Form enthält. |
| [GetShadowEffect](./getshadoweffect/) | Stellt ein Drawing.ShadowEffect‑Objekt dar, das den Schatteneffekt für das Diagrammelement oder die Form angibt. |
| [GetReflection](./getreflection/) | Stellt ein ReflectionEffect‑Objekt dar, das den Reflexionseffekt für das Diagrammelement oder die Form angibt. |
| [GetGlow](./getglow/) | Stellt ein GlowEffect‑Objekt dar, das den Leuchteffekt für das Diagrammelement oder die Form angibt. |
| [GetSoftEdges](./getsoftedges/) | Liest und setzt den Radius der Unschärfe, die auf die Kanten angewendet wird, in Punkten. |
| [SetSoftEdges](./setsoftedges/) | Liest und setzt den Radius der Unschärfe, die auf die Kanten angewendet wird, in Punkten. |
| [GetThreeDFormat](./getthreedformat/) | Liest und setzt das 3D‑Format der Form. |
| [GetFormatPicture](./getformatpicture/) | Liest und setzt die Optionen des Bildformats. |
| [IsHidden](./ishidden/) | Gibt an, ob das Objekt sichtbar ist. |
| [SetIsHidden](./setishidden/) | Gibt an, ob das Objekt sichtbar ist. |
| [IsAspectRatioLocked](./isaspectratiolocked/) | True bedeutet, dass das Seitenverhältnis der Form gesperrt ist. |
| [SetIsAspectRatioLocked](./setisaspectratiolocked/) | True bedeutet, dass das Seitenverhältnis der Form gesperrt ist. |
| [GetLockedProperty](./getlockedproperty/) | Liest den Wert der gesperrten Eigenschaft. |
| [SetLockedProperty](./setlockedproperty/) | Setzt die gesperrte Eigenschaft. |
| [GetRotationAngle](./getrotationangle/) | Liest und setzt die Drehung der Form. |
| [SetRotationAngle](./setrotationangle/) | Liest und setzt die Drehung der Form. |
| [AddHyperlink](./addhyperlink/) | Fügt der Form einen Hyperlink hinzu. |
| [RemoveHyperlink](./removehyperlink/) | Entfernt den Hyperlink der Form. |
| [GetHyperlink](./gethyperlink/) | Liest den Hyperlink der Form. |
| [MoveToRange](./movetorange/) | Verschiebt die Form in einen angegebenen Bereich. |
| [AlignTopRightCorner](./aligntoprightcorner/) | Verschiebt das Bild in die obere rechte Ecke. |
| [GetId](./getid/) | Liest die Kennung dieser Form. |
| [GetSpid](./getspid/) | Legt einen optionalen Zeichenkettenbezeichner fest, den eine Anwendung verwenden kann, um die bestimmte Form zu identifizieren. |
| [GetSpt](./getspt/) | Legt eine optionale Nummer fest, die eine Anwendung verwenden kann, um die bestimmte Form einem definierten Formtyp zuzuordnen. |
| [GetWorksheet](./getworksheet/) | Ruft das Aspose.Cells.Worksheet-Objekt ab, das dieses Shape enthält. |
| [IsGroup](./isgroup/) | Gibt an, ob dieses Shape ein Gruppenshape ist. |
| [IsInGroup](./isingroup/) | Gibt an, ob das Shape gruppiert ist. |
| [IsWordArt](./iswordart/) | Gibt an, ob dieses Shape ein WordArt ist. |
| [GetTextEffect](./gettexteffect/) | Gibt ein TextEffectFormat-Objekt zurück, das Text-Effekt-Formatierungseigenschaften für das angegebene Shape enthält. Gilt für Shape-Objekte, die WordArt darstellen. |
| [IsLocked](./islocked/) | True bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. Beachten Sie, dass dieser Wert nur sinnvoll ist, wenn das Arbeitsblatt oder die Objekte im Arbeitsblatt geschützt sind. |
| [SetIsLocked](./setislocked/) | True bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. Beachten Sie, dass dieser Wert nur sinnvoll ist, wenn das Arbeitsblatt oder die Objekte im Arbeitsblatt geschützt sind. |
| [IsPrintable](./isprintable/) | Gibt an, ob das Objekt druckbar ist. Wenn False, wird dieses Shape beim Drucken nicht ausgegeben. |
| [SetIsPrintable](./setisprintable/) | Gibt an, ob das Objekt druckbar ist. Wenn False, wird dieses Shape beim Drucken nicht ausgegeben. |
| [GetMsoDrawingType](./getmsodrawingtype/) | Ruft den Zeichnungstyp ab. |
| [GetAutoShapeType](./getautoshapetype/) | Ruft den AutoShape-Typ ab und legt ihn fest. |
| [SetAutoShapeType](./setautoshapetype/) | Ruft den AutoShape-Typ ab und legt ihn fest. |
| [GetAnchorType](./getanchortype/) | Ruft den Typ des Shape-Anker-Platzhalters ab und legt ihn fest. |
| [SetAnchorType](./setanchortype/) | Ruft den Typ des Shape-Anker-Platzhalters ab und legt ihn fest. |
| [GetPlacement](./getplacement/) | Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die Eigenschaft steuert die Platzierung eines Objekts auf einem Arbeitsblatt. |
| [SetPlacement](./setplacement/) | Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die Eigenschaft steuert die Platzierung eines Objekts auf einem Arbeitsblatt. |
| [GetUpperLeftRow](./getupperleftrow/) | Stellt den Index der obersten Zeile dar. |
| [SetUpperLeftRow](./setupperleftrow/) | Stellt den Index der obersten Zeile dar. |
| [GetUpperDeltaY](./getupperdeltay/) | Ruft den vertikalen Versatz des Shapes von seiner oberen linken Zeilenposition ab oder legt ihn fest. |
| [SetUpperDeltaY](./setupperdeltay/) | Ruft den vertikalen Versatz des Shapes von seiner oberen linken Zeilenposition ab oder legt ihn fest. |
| [GetUpperLeftColumn](./getupperleftcolumn/) | Stellt den Spaltenindex der oberen linken Ecke dar. |
| [SetUpperLeftColumn](./setupperleftcolumn/) | Stellt den Spaltenindex der oberen linken Ecke dar. |
| [GetUpperDeltaX](./getupperdeltax/) | Ruft den horizontalen Versatz des Shapes von seiner oberen linken Spaltenposition ab oder legt ihn fest. |
| [SetUpperDeltaX](./setupperdeltax/) | Ruft den horizontalen Versatz des Shapes von seiner oberen linken Spaltenposition ab oder legt ihn fest. |
| [GetLowerRightRow](./getlowerrightrow/) | Stellt den Zeilenindex der unteren rechten Ecke dar. |
| [SetLowerRightRow](./setlowerrightrow/) | Stellt den Zeilenindex der unteren rechten Ecke dar. |
| [GetLowerDeltaY](./getlowerdeltay/) | Ruft den vertikalen Versatz des Shapes von seiner unteren rechten Zeilenposition ab oder legt ihn fest. |
| [SetLowerDeltaY](./setlowerdeltay/) | Ruft den vertikalen Versatz des Shapes von seiner unteren rechten Zeilenposition ab oder legt ihn fest. |
| [GetLowerRightColumn](./getlowerrightcolumn/) | Stellt den Spaltenindex der unteren rechten Ecke dar. |
| [SetLowerRightColumn](./setlowerrightcolumn/) | Stellt den Spaltenindex der unteren rechten Ecke dar. |
| [GetLowerDeltaX](./getlowerdeltax/) | Ruft den horizontalen Versatz des Shapes von seiner unteren rechten Spaltenposition ab oder legt ihn fest. |
| [SetLowerDeltaX](./setlowerdeltax/) | Ruft den horizontalen Versatz des Shapes von seiner unteren rechten Spaltenposition ab oder legt ihn fest. |
| [GetRight](./getright/) | Stellt die Breite des horizontalen Versatzes des Shapes von seiner unteren rechten Spaltenposition in Pixeln dar. |
| [SetRight](./setright/) | Stellt die Breite des horizontalen Versatzes des Shapes von seiner unteren rechten Spaltenposition in Pixeln dar. |
| [GetBottom](./getbottom/) | Stellt die Breite des vertikalen Versatzes des Shapes von seiner unteren rechten Zeilenposition in Pixeln dar. |
| [SetBottom](./setbottom/) | Stellt die Breite des vertikalen Versatzes des Shapes von seiner unteren rechten Zeilenposition in Pixeln dar. |
| [GetWidth](./getwidth/) | Stellt die Breite des Shapes in Pixeln dar. |
| [SetWidth](./setwidth/) | Stellt die Breite des Shapes in Pixeln dar. |
| [GetWidthInch](./getwidthinch/) | Stellt die Breite des Shapes in Zoll dar. |
| [SetWidthInch](./setwidthinch/) | Stellt die Breite des Shapes in Zoll dar. |
| [GetWidthPt](./getwidthpt/) | Stellt die Breite des Shapes in Punkt dar. |
| [SetWidthPt](./setwidthpt/) | Stellt die Breite des Shapes in Punkt dar. |
| [GetWidthCM](./getwidthcm/) | Stellt die Breite des Shapes in Zentimetern dar. |
| [SetWidthCM](./setwidthcm/) | Stellt die Breite des Shapes in Zentimetern dar. |
| [GetHeight](./getheight/) | Stellt die Höhe der Form dar, in Einheit Pixel. |
| [SetHeight](./setheight/) | Stellt die Höhe der Form dar, in Einheit Pixel. |
| [GetHeightInch](./getheightinch/) | Stellt die Höhe der Form dar, in Einheit Zoll. |
| [SetHeightInch](./setheightinch/) | Stellt die Höhe der Form dar, in Einheit Zoll. |
| [GetHeightPt](./getheightpt/) | Stellt die Höhe der Form dar, in Einheit Punkt. |
| [SetHeightPt](./setheightpt/) | Stellt die Höhe der Form dar, in Einheit Punkt. |
| [GetHeightCM](./getheightcm/) | Stellt die Höhe der Form dar, in Einheit Zentimeter. |
| [SetHeightCM](./setheightcm/) | Stellt die Höhe der Form dar, in Einheit Zentimeter. |
| [GetLeft](./getleft/) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheit Pixel. |
| [SetLeft](./setleft/) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheit Pixel. |
| [GetLeftInch](./getleftinch/) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheit Zoll. |
| [SetLeftInch](./setleftinch/) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheit Zoll. |
| [GetLeftCM](./getleftcm/) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheit Zentimeter. |
| [SetLeftCM](./setleftcm/) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheit Zentimeter. |
| [GetTop](./gettop/) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in Einheit Pixel. |
| [SetTop](./settop/) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in Einheit Pixel. |
| [GetTopInch](./gettopinch/) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in Einheit Zoll. |
| [SetTopInch](./settopinch/) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in Einheit Zoll. |
| [GetTopCM](./gettopcm/) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in Einheit Zentimeter. |
| [SetTopCM](./settopcm/) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in Einheit Zentimeter. |
| [GetTopToCorner](./gettoptocorner/) | Liest und setzt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel. |
| [SetTopToCorner](./settoptocorner/) | Liest und setzt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel. |
| [GetLeftToCorner](./getlefttocorner/) | Liest und setzt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts. |
| [SetLeftToCorner](./setlefttocorner/) | Liest und setzt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts. |
| [GetX](./getx/) | Liest und setzt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts, in Einheit Pixel. |
| [SetX](./setx/) | Liest und setzt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts, in Einheit Pixel. |
| [GetY](./gety/) | Liest und setzt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel. |
| [SetY](./sety/) | Liest und setzt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel. |
| [GetWidthScale](./getwidthscale/) | Liest und setzt die Breiten‑Skalierung, in Prozent der ursprünglichen Bildbreite. Wenn die Form kein Bild ist, gibt die WidthScale‑Eigenschaft nur 100 zurück; |
| [SetWidthScale](./setwidthscale/) | Liest und setzt die Breiten‑Skalierung, in Prozent der ursprünglichen Bildbreite. Wenn die Form kein Bild ist, gibt die WidthScale‑Eigenschaft nur 100 zurück; |
| [GetHeightScale](./getheightscale/) | Liest und setzt die Höhen‑Skalierung, in Prozent der ursprünglichen Bildhöhe. Wenn die Form kein Bild ist, gibt die HeightScale‑Eigenschaft nur 100 zurück; |
| [SetHeightScale](./setheightscale/) | Liest und setzt die Höhen‑Skalierung, in Prozent der ursprünglichen Bildhöhe. Wenn die Form kein Bild ist, gibt die HeightScale‑Eigenschaft nur 100 zurück; |
| [GetTopInShape](./gettopinshape/) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form dar, in 1/4000 der Höhe der übergeordneten Form. |
| [SetTopInShape](./settopinshape/) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form dar, in 1/4000 der Höhe der übergeordneten Form. |
| [GetLeftInShape](./getleftinshape/) | Stellt den horizontalen Versatz der Form vom linken Rand der übergeordneten Form dar, in 1/4000 der Breite der übergeordneten Form. |
| [SetLeftInShape](./setleftinshape/) | Stellt den horizontalen Versatz der Form vom linken Rand der übergeordneten Form dar, in 1/4000 der Breite der übergeordneten Form. |
| [GetWidthInShape](./getwidthinshape/) | Stellt die Breite der Form dar, in 1/4000 der übergeordneten Form. |
| [SetWidthInShape](./setwidthinshape/) | Stellt die Breite der Form dar, in 1/4000 der übergeordneten Form. |
| [GetHeightInShape](./getheightinshape/) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form dar, in 1/4000 der Höhe der übergeordneten Form.. |
| [SetHeightInShape](./setheightinshape/) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form dar, in 1/4000 der Höhe der übergeordneten Form.. |
| [GetGroup](./getgroup/) | Liest die Gruppierungsform, die diese Form enthält. |
| [GetType](./gettype/) | Liest den AutoForm‑Typ. |
| [GetHasLine](./gethasline/) | Liest und setzt, ob die Linienumrandung der Form sichtbar ist. |
| [SetHasLine](./sethasline/) | Liest und setzt, ob die Linienumrandung der Form sichtbar ist. |
| [IsFilled](./isfilled/) | Gibt an, ob das Füllformat sichtbar ist. |
| [SetIsFilled](./setisfilled/) | Gibt an, ob das Füllformat sichtbar ist. |
| [IsFlippedHorizontally](./isflippedhorizontally/) | Liest und setzt, ob die Form horizontal gespiegelt ist. |
| [SetIsFlippedHorizontally](./setisflippedhorizontally/) | Liest und setzt, ob die Form horizontal gespiegelt ist. |
| [IsFlippedVertically](./isflippedvertically/) | Liest und schreibt, ob die Form vertikal gespiegelt ist. |
| [SetIsFlippedVertically](./setisflippedvertically/) | Liest und schreibt, ob die Form vertikal gespiegelt ist. |
| [GetActualLowerRightRow](./getactuallowerrightrow/) | Ruft die tatsächliche unterste Zeile ab. |
| [GetConnectionPoints](./getconnectionpoints/) | Ruft die Verbindungspunkte ab. |
| [ToImage_ImageType](./toimage_imagetype/) | Erstellt das Formbild und speichert es in einem Stream im angegebenen Format. |
| [GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | Gibt an, ob die Form relativ zur Originalbildgröße ist. |
| [SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | Gibt an, ob die Form relativ zur Originalbildgröße ist. |
| [GetLinkedCell](./getlinkedcell/) | Liest oder schreibt den Arbeitsblattbereich, der mit dem Wert des Steuerelements verknüpft ist. |
| [SetLinkedCell_String](./setlinkedcell_string/) | Liest oder schreibt den Arbeitsblattbereich, der mit dem Wert des Steuerelements verknüpft ist. |
| [GetInputRange](./getinputrange/) | Liest oder schreibt den Arbeitsblattbereich, der zum Befüllen der angegebenen Kombinationsbox verwendet wird. |
| [SetInputRange_String](./setinputrange_string/) | Liest oder schreibt den Arbeitsblattbereich, der zum Befüllen der angegebenen Kombinationsbox verwendet wird. |
| [UpdateSelectedValue](./updateselectedvalue/) | Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle. |
| [GetTextShapeType](./gettextshapetype/) | Liest und schreibt den voreingestellten Textformtyp. |
| [SetTextShapeType](./settextshapetype/) | Liest und schreibt den voreingestellten Textformtyp. |
| [GetTextBody](./gettextbody/) | Liest und schreibt die Einstellung des Textes der Form. |
| [GetFont](./getfont/) | Stellt die Schriftart der Form dar. |
| [SetFont](./setfont/) | Stellt die Schriftart der Form dar. |
| [GetTextOptions](./gettextoptions/) | Stellt die Textoptionen der Form dar. |
| [SetTextOptions](./settextoptions/) | Stellt die Textoptionen der Form dar. |
| [CalculateTextSize](./calculatetextsize/) | Berechnet den Textbereich neu. |
| [GetText](./gettext/) | Liest und schreibt den Text dieser Form. |
| [SetText](./settext/) | Liest und schreibt den Text dieser Form. |
| [IsRichText](./isrichtext/) | Gibt an, ob der Text Rich Text ist oder nicht. |
| [GetHtmlText](./gethtmltext/) | Liest und schreibt die HTML-Zeichenkette, die Daten und einige Formate in diesem Textfeld enthält. |
| [SetHtmlText](./sethtmltext/) | Liest und schreibt die HTML-Zeichenkette, die Daten und einige Formate in diesem Textfeld enthält. |
| [FormatCharacters](./formatcharacters/) | Formatiert einige Zeichen mit den Schriftarteinstellungen. |
| [Characters](./characters/) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich innerhalb des Textes darstellt. |
| [GetRichFormattings](./getrichformattings/) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich innerhalb des Textes darstellen. |
| [GetTextVerticalOverflow](./gettextverticaloverflow/) | Liest und schreibt den vertikalen Überlauftyp des Textes der Form, die Text enthält. |
| [SetTextVerticalOverflow](./settextverticaloverflow/) | Liest und schreibt den vertikalen Überlauftyp des Textes der Form, die Text enthält. |
| [GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | Liest und schreibt den horizontalen Überlauftyp des Textes der Form, die Text enthält. |
| [SetTextHorizontalOverflow](./settexthorizontaloverflow/) | Liest und schreibt den horizontalen Überlauftyp des Textes der Form, die Text enthält. |
| [IsTextWrapped](./istextwrapped/) | Liest und schreibt den Zeilenumbruchtyp des Textes der Form, die Text enthält. |
| [SetIsTextWrapped](./setistextwrapped/) | Liest und schreibt den Zeilenumbruchtyp des Textes der Form, die Text enthält. |
| [GetTextOrientationType](./gettextorientationtype/) | Liest und schreibt den Textausrichtungstyp der Form. |
| [SetTextOrientationType](./settextorientationtype/) | Liest und schreibt den Textausrichtungstyp der Form. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Liest und schreibt den horizontalen Ausrichtungstyp des Textes der Form. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Liest und schreibt den horizontalen Ausrichtungstyp des Textes der Form. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Liest und schreibt den vertikalen Ausrichtungstyp des Textes der Form. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Liest und schreibt den vertikalen Ausrichtungstyp des Textes der Form. |
| [GetTextDirection](./gettextdirection/) | Liest/Setzt die Richtung des Textflusses für dieses Objekt. |
| [SetTextDirection](./settextdirection/) | Liest/Setzt die Richtung des Textflusses für dieses Objekt. |
| [GetTextBoxOptions](./gettextboxoptions/) | Liest die Textinformationen in der Form |
| [GetControlData](./getcontroldata/) | Liest die Daten des Steuerelements. |
| [GetActiveXControl](./getactivexcontrol/) | Liest das ActiveX-Steuerelement. |
| [RemoveActiveXControl](./removeactivexcontrol/) | Entferne das ActiveX-Steuerelement. |
| [GetPaths](./getpaths/) | Liest die Pfade einer benutzerdefinierten geometrischen Form. |
| [GetGeometry](./getgeometry/) | Liest die Geometrie |
| [GetCreateId](./getcreateid/) | Liest und setzt die Erstellungs-ID für diese Form. |
| [SetCreateId](./setcreateid/) | Liest und setzt die Erstellungs-ID für diese Form. |
| [IsDecorative](./isdecorative/) | Gibt an, ob das Objekt dekorativ ist. |
| [SetIsDecorative](./setisdecorative/) | Gibt an, ob das Objekt dekorativ ist. |
| [GetActualBox](./getactualbox/) | Lese die tatsächliche Position und Größe der Form (nach Anwendung von Drehung, Spiegelung usw.). |
| [FitToTextSize](./fittotextsize/) | Berechne einen Textbereich neu, der geeignet ist, den gesamten Textinhalt anzuzeigen. |
| [IsSameSetting](./issamesetting/) | Gibt zurück, ob die Form identisch ist. |
