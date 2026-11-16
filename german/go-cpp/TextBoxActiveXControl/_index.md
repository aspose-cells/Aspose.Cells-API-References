---
title: "TextBoxActiveXControl Class"
linktitle: "TextBoxActiveXControl"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "TextBoxActiveXControl-Klasse. Kapselt das Objekt, das textboxactivexcontrol in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/textboxactivexcontrol/
---

## TextBoxActiveXControl class

Stellt ein Textfeld-ActiveX-Steuerelement dar.

```go

type TextBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewTextBoxActiveXControl](./newtextboxactivexcontrol/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetType](./gettype/) | Liest den Typ des ActiveX-Steuerelements. |
| [GetBorderStyle](./getborderstyle/) | Liest und setzt den von dem Steuerelement verwendeten Rahmentyp. |
| [SetBorderStyle](./setborderstyle/) | Liest und setzt den von dem Steuerelement verwendeten Rahmentyp. |
| [GetBorderOleColor](./getborderolecolor/) | Liest und legt die OLE-Farbe des Hintergrunds fest. |
| [SetBorderOleColor](./setborderolecolor/) | Liest und legt die OLE-Farbe des Hintergrunds fest. |
| [GetSpecialEffect](./getspecialeffect/) | Liest und setzt den Spezialeffekt des Steuerelements. |
| [SetSpecialEffect](./setspecialeffect/) | Liest und setzt den Spezialeffekt des Steuerelements. |
| [GetMaxLength](./getmaxlength/) | Liest und setzt die maximale Anzahl von Zeichen |
| [SetMaxLength](./setmaxlength/) | Liest und setzt die maximale Anzahl von Zeichen |
| [GetScrollBars](./getscrollbars/) | Gibt an, ob das Steuerelement vertikale Bildlaufleisten, horizontale Bildlaufleisten, beides oder keines davon hat. |
| [SetScrollBars](./setscrollbars/) | Gibt an, ob das Steuerelement vertikale Bildlaufleisten, horizontale Bildlaufleisten, beides oder keines davon hat. |
| [GetPasswordChar](./getpasswordchar/) | Liest und setzt ein Zeichen, das anstelle der eingegebenen Zeichen angezeigt wird. |
| [SetPasswordChar](./setpasswordchar/) | Liest und setzt ein Zeichen, das anstelle der eingegebenen Zeichen angezeigt wird. |
| [IsEditable](./iseditable/) | Gibt an, ob der Benutzer in das Steuerelement tippen kann. |
| [SetIsEditable](./setiseditable/) | Gibt an, ob der Benutzer in das Steuerelement tippen kann. |
| [GetIntegralHeight](./getintegralheight/) | Gibt an, ob das Steuerelement nur vollständige Textzeilen anzeigt, ohne Teilzeilen darzustellen. |
| [SetIntegralHeight](./setintegralheight/) | Gibt an, ob das Steuerelement nur vollständige Textzeilen anzeigt, ohne Teilzeilen darzustellen. |
| [IsDragBehaviorEnabled](./isdragbehaviorenabled/) | Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist. |
| [SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist. |
| [GetEnterKeyBehavior](./getenterkeybehavior/) | Gibt das Verhalten der ENTER-Taste an. True gibt an, dass das Drücken von ENTER eine neue Zeile erzeugt. False gibt an, dass das Drücken von ENTER den Fokus zum nächsten Objekt in der Tab-Reihenfolge verschiebt. |
| [SetEnterKeyBehavior](./setenterkeybehavior/) | Gibt das Verhalten der ENTER-Taste an. True gibt an, dass das Drücken von ENTER eine neue Zeile erzeugt. False gibt an, dass das Drücken von ENTER den Fokus zum nächsten Objekt in der Tab-Reihenfolge verschiebt. |
| [GetEnterFieldBehavior](./getenterfieldbehavior/) | Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True gibt an, dass die Auswahl unverändert bleibt seit dem letzten Mal, als das Steuerelement aktiv war. False gibt an, dass der gesamte Text im Steuerelement beim Betreten ausgewählt wird. |
| [SetEnterFieldBehavior](./setenterfieldbehavior/) | Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True gibt an, dass die Auswahl unverändert bleibt seit dem letzten Mal, als das Steuerelement aktiv war. False gibt an, dass der gesamte Text im Steuerelement beim Betreten ausgewählt wird. |
| [GetTabKeyBehavior](./gettabkeybehavior/) | Gibt an, ob Tabulatorzeichen im Text des Steuerelements erlaubt sind. |
| [SetTabKeyBehavior](./settabkeybehavior/) | Gibt an, ob Tabulatorzeichen im Text des Steuerelements erlaubt sind. |
| [GetHideSelection](./gethideselection/) | Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat. |
| [SetHideSelection](./sethideselection/) | Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat. |
| [IsAutoTab](./isautotab/) | Gibt an, ob der Fokus automatisch zum nächsten Steuerelement wechselt, wenn der Benutzer die maximale Zeichenanzahl eingibt. |
| [SetIsAutoTab](./setisautotab/) | Gibt an, ob der Fokus automatisch zum nächsten Steuerelement wechselt, wenn der Benutzer die maximale Zeichenanzahl eingibt. |
| [IsMultiLine](./ismultiline/) | Gibt an, ob das Steuerelement mehr als eine Textzeile anzeigen kann. |
| [SetIsMultiLine](./setismultiline/) | Gibt an, ob das Steuerelement mehr als eine Textzeile anzeigen kann. |
| [IsWordWrapped](./iswordwrapped/) | Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird. |
| [SetIsWordWrapped](./setiswordwrapped/) | Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird. |
| [GetText](./gettext/) | Liest und setzt den Text des Steuerelements. |
| [SetText](./settext/) | Liest und setzt den Text des Steuerelements. |
| [GetDropButtonStyle](./getdropbuttonstyle/) | Gibt das Symbol an, das auf der Dropdown‑Schaltfläche angezeigt wird |
| [SetDropButtonStyle](./setdropbuttonstyle/) | Gibt das Symbol an, das auf der Dropdown‑Schaltfläche angezeigt wird |
| [GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | Gibt das Symbol an, das auf der Dropdown‑Schaltfläche angezeigt wird |
| [SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | Gibt das Symbol an, das auf der Dropdown‑Schaltfläche angezeigt wird |
| [IsAutoWordSelected](./isautowordselected/) | Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist. |
| [SetIsAutoWordSelected](./setisautowordselected/) | Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist. |
| [IsEnabled](./isenabled/) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [SetIsEnabled](./setisenabled/) | Gibt an, ob das Steuerelement den Fokus erhalten und auf benutzergenerierte Ereignisse reagieren kann. |
| [IsLocked](./islocked/) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [SetIsLocked](./setislocked/) | Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind. |
| [IsTransparent](./istransparent/) | Gibt an, ob das Steuerelement transparent ist. |
| [SetIsTransparent](./setistransparent/) | Gibt an, ob das Steuerelement transparent ist. |
| [GetIMEMode](./getimemode/) | Liest und schreibt den Standard‑Laufzeitmodus des Eingabemethoden‑Editors für das Steuerelement, wenn es den Fokus erhält. |
| [SetIMEMode](./setimemode/) | Liest und schreibt den Standard‑Laufzeitmodus des Eingabemethoden‑Editors für das Steuerelement, wenn es den Fokus erhält. |
| [GetFont](./getfont/) | Stellt die Schriftart des Steuerelements dar. |
| [GetTextAlign](./gettextalign/) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [SetTextAlign](./settextalign/) | Stellt dar, wie der vom Steuerelement verwendete Text ausgerichtet wird. |
| [GetData](./getdata/) | Liest und legt die Binärdaten des Steuerelements fest. |
| [IsAutoSize](./isautosize/) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [SetIsAutoSize](./setisautosize/) | Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen. |
| [GetWorkbook](./getworkbook/) | Liest das Workbook-Objekt. |
| [GetMouseIcon](./getmouseicon/) | Liest und legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [SetMouseIcon](./setmouseicon/) | Liest und legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [GetMousePointer](./getmousepointer/) | Liest und legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [SetMousePointer](./setmousepointer/) | Liest und legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [GetLinkedCell](./getlinkedcell/) | Liest und legt die verknüpfte Zelle fest. |
| [SetLinkedCell](./setlinkedcell/) | Liest und legt die verknüpfte Zelle fest. |
| [GetListFillRange](./getlistfillrange/) | Liest und legt den Listenfüllbereich fest. |
| [SetListFillRange](./setlistfillrange/) | Liest und legt den Listenfüllbereich fest. |
| [GetWidth](./getwidth/) | Liest und legt die Breite des Steuerelements in Punkt-Einheiten fest. |
| [SetWidth](./setwidth/) | Liest und legt die Breite des Steuerelements in Punkt-Einheiten fest. |
| [GetHeight](./getheight/) | Liest und legt die Höhe des Steuerelements in Punkt-Einheiten fest. |
| [SetHeight](./setheight/) | Liest und legt die Höhe des Steuerelements in Punkt-Einheiten fest. |
| [GetForeOleColor](./getforeolecolor/) | Liest und legt die OLE-Farbe des Vordergrunds fest. |
| [SetForeOleColor](./setforeolecolor/) | Liest und legt die OLE-Farbe des Vordergrunds fest. |
| [GetBackOleColor](./getbackolecolor/) | Liest und legt die OLE-Farbe des Hintergrunds fest. |
| [SetBackOleColor](./setbackolecolor/) | Liest und legt die OLE-Farbe des Hintergrunds fest. |
| [IsVisible](./isvisible/) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [SetIsVisible](./setisvisible/) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [GetShadow](./getshadow/) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [SetShadow](./setshadow/) | Gibt an, ob ein Schatten angezeigt werden soll. |
