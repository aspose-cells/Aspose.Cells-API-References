---
title: "TextBoxActiveXControl Klass"
linktitle: "TextBoxActiveXControl"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "TextBoxActiveXControl klass. Inkapslar objektet som representerar textboxactivexcontrol i Go."
type: docs
weight: 200
url: /sv/go-cpp/textboxactivexcontrol/
---

## TextBoxActiveXControl class

Representerar en textfält‑ActiveX‑kontroll.

```go

type TextBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewTextBoxActiveXControl](./newtextboxactivexcontrol/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetType](./gettype/) | Hämtar typen av ActiveX-kontrollen. |
| [GetBorderStyle](./getborderstyle/) | Hämtar och anger typen av ram som används av kontrollen. |
| [SetBorderStyle](./setborderstyle/) | Hämtar och anger typen av ram som används av kontrollen. |
| [GetBorderOleColor](./getborderolecolor/) | Hämtar och anger OLE-färgen för bakgrunden. |
| [SetBorderOleColor](./setborderolecolor/) | Hämtar och anger OLE-färgen för bakgrunden. |
| [GetSpecialEffect](./getspecialeffect/) | Hämtar och anger den speciella effekten för kontrollen. |
| [SetSpecialEffect](./setspecialeffect/) | Hämtar och anger den speciella effekten för kontrollen. |
| [GetMaxLength](./getmaxlength/) | Hämtar och anger det maximala antalet tecken |
| [SetMaxLength](./setmaxlength/) | Hämtar och anger det maximala antalet tecken |
| [GetScrollBars](./getscrollbars/) | Anger om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen. |
| [SetScrollBars](./setscrollbars/) | Anger om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen. |
| [GetPasswordChar](./getpasswordchar/) | Hämtar och sätter ett tecken som ska visas i stället för de inmatade tecknen. |
| [SetPasswordChar](./setpasswordchar/) | Hämtar och sätter ett tecken som ska visas i stället för de inmatade tecknen. |
| [IsEditable](./iseditable/) | Anger om användaren kan skriva i kontrollen. |
| [SetIsEditable](./setiseditable/) | Anger om användaren kan skriva i kontrollen. |
| [GetIntegralHeight](./getintegralheight/) | Anger om kontrollen endast visar kompletta textrader utan att visa några partiella rader. |
| [SetIntegralHeight](./setintegralheight/) | Anger om kontrollen endast visar kompletta textrader utan att visa några partiella rader. |
| [IsDragBehaviorEnabled](./isdragbehaviorenabled/) | Anger om dra-och-släpp är aktiverat för kontrollen. |
| [SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | Anger om dra-och-släpp är aktiverat för kontrollen. |
| [GetEnterKeyBehavior](./getenterkeybehavior/) | Anger beteendet för ENTER-tangenten.True anger att trycka på ENTER skapar en ny rad.False anger att trycka på ENTER flyttar fokus till nästa objekt i tabb-ordningen. |
| [SetEnterKeyBehavior](./setenterkeybehavior/) | Anger beteendet för ENTER-tangenten.True anger att trycka på ENTER skapar en ny rad.False anger att trycka på ENTER flyttar fokus till nästa objekt i tabb-ordningen. |
| [GetEnterFieldBehavior](./getenterfieldbehavior/) | Anger urvalsbeteendet när kontrollen aktiveras. True anger att urvalet förblir oförändrat från senaste gången kontrollen var aktiv. False anger att all text i kontrollen kommer att markeras när kontrollen aktiveras. |
| [SetEnterFieldBehavior](./setenterfieldbehavior/) | Anger urvalsbeteendet när kontrollen aktiveras. True anger att urvalet förblir oförändrat från senaste gången kontrollen var aktiv. False anger att all text i kontrollen kommer att markeras när kontrollen aktiveras. |
| [GetTabKeyBehavior](./gettabkeybehavior/) | Indikerar om tabbtecken är tillåtna i kontrollens text. |
| [SetTabKeyBehavior](./settabkeybehavior/) | Indikerar om tabbtecken är tillåtna i kontrollens text. |
| [GetHideSelection](./gethideselection/) | Anger om markerad text i kontrollen visas som markerad när kontrollen inte har fokus. |
| [SetHideSelection](./sethideselection/) | Anger om markerad text i kontrollen visas som markerad när kontrollen inte har fokus. |
| [IsAutoTab](./isautotab/) | Indikerar om fokus automatiskt kommer att flyttas till nästa kontroll när användaren anger det maximala antalet tecken. |
| [SetIsAutoTab](./setisautotab/) | Indikerar om fokus automatiskt kommer att flyttas till nästa kontroll när användaren anger det maximala antalet tecken. |
| [IsMultiLine](./ismultiline/) | Indikerar om kontrollen kan visa mer än en rad text. |
| [SetIsMultiLine](./setismultiline/) | Indikerar om kontrollen kan visa mer än en rad text. |
| [IsWordWrapped](./iswordwrapped/) | Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad. |
| [SetIsWordWrapped](./setiswordwrapped/) | Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad. |
| [GetText](./gettext/) | Hämtar och sätter texten i kontrollen. |
| [SetText](./settext/) | Hämtar och sätter texten i kontrollen. |
| [GetDropButtonStyle](./getdropbuttonstyle/) | Anger symbolen som visas på nedrullningsknappen. |
| [SetDropButtonStyle](./setdropbuttonstyle/) | Anger symbolen som visas på nedrullningsknappen. |
| [GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | Anger symbolen som visas på nedrullningsknappen. |
| [SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | Anger symbolen som visas på nedrullningsknappen. |
| [IsAutoWordSelected](./isautowordselected/) | Anger den grundläggande enheten som används för att utöka ett urval. True anger att den grundläggande enheten är ett enskilt tecken. false anger att den grundläggande enheten är ett helt ord. |
| [SetIsAutoWordSelected](./setisautowordselected/) | Anger den grundläggande enheten som används för att utöka ett urval. True anger att den grundläggande enheten är ett enskilt tecken. false anger att den grundläggande enheten är ett helt ord. |
| [IsEnabled](./isenabled/) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [SetIsEnabled](./setisenabled/) | Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser. |
| [IsLocked](./islocked/) | Anger om data i kontrollen är låst för redigering. |
| [SetIsLocked](./setislocked/) | Anger om data i kontrollen är låst för redigering. |
| [IsTransparent](./istransparent/) | Anger om kontrollen är transparent. |
| [SetIsTransparent](./setistransparent/) | Anger om kontrollen är transparent. |
| [GetIMEMode](./getimemode/) | Hämtar och anger standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [SetIMEMode](./setimemode/) | Hämtar och anger standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus. |
| [GetFont](./getfont/) | Representerar kontrollens teckensnitt. |
| [GetTextAlign](./gettextalign/) | Representerar hur texten som används av kontrollen ska justeras. |
| [SetTextAlign](./settextalign/) | Representerar hur texten som används av kontrollen ska justeras. |
| [GetData](./getdata/) | Hämtar och anger kontrollens binära data. |
| [IsAutoSize](./isautosize/) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela sitt innehåll. |
| [SetIsAutoSize](./setisautosize/) | Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela sitt innehåll. |
| [GetWorkbook](./getworkbook/) | Hämtar Workbook-objektet. |
| [GetMouseIcon](./getmouseicon/) | Hämtar och anger en anpassad ikon som ska visas som muspekaren för kontrollen. |
| [SetMouseIcon](./setmouseicon/) | Hämtar och anger en anpassad ikon som ska visas som muspekaren för kontrollen. |
| [GetMousePointer](./getmousepointer/) | Hämtar och anger typen av ikon som visas som muspekaren för kontrollen. |
| [SetMousePointer](./setmousepointer/) | Hämtar och anger typen av ikon som visas som muspekaren för kontrollen. |
| [GetLinkedCell](./getlinkedcell/) | Hämtar och anger den länkade cellen. |
| [SetLinkedCell](./setlinkedcell/) | Hämtar och anger den länkade cellen. |
| [GetListFillRange](./getlistfillrange/) | Hämtar och anger listans fyllningsintervall. |
| [SetListFillRange](./setlistfillrange/) | Hämtar och anger listans fyllningsintervall. |
| [GetWidth](./getwidth/) | Hämtar och anger kontrollens bredd i enheter av punkter. |
| [SetWidth](./setwidth/) | Hämtar och anger kontrollens bredd i enheter av punkter. |
| [GetHeight](./getheight/) | Hämtar och anger kontrollens höjd i enheter av punkter. |
| [SetHeight](./setheight/) | Hämtar och anger kontrollens höjd i enheter av punkter. |
| [GetForeOleColor](./getforeolecolor/) | Hämtar och anger OLE-färgen för förgrunden. |
| [SetForeOleColor](./setforeolecolor/) | Hämtar och anger OLE-färgen för förgrunden. |
| [GetBackOleColor](./getbackolecolor/) | Hämtar och anger OLE-färgen för bakgrunden. |
| [SetBackOleColor](./setbackolecolor/) | Hämtar och anger OLE-färgen för bakgrunden. |
| [IsVisible](./isvisible/) | Indikerar om denna kontroll är synlig. |
| [SetIsVisible](./setisvisible/) | Indikerar om denna kontroll är synlig. |
| [GetShadow](./getshadow/) | Indikerar om en skugga ska visas. |
| [SetShadow](./setshadow/) | Indikerar om en skugga ska visas. |
