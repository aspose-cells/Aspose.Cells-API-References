---
title: "TextBoxActiveXControl Class"
linktitle: "TextBoxActiveXControl"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "TextBoxActiveXControl class. Incapsula l'oggetto che rappresenta textboxactivexcontrol in Go."
type: docs
weight: 200
url: /it/go-cpp/textboxactivexcontrol/
---

## TextBoxActiveXControl class

Rappresenta un controllo ActiveX casella di testo.

```go

type TextBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewTextBoxActiveXControl](./newtextboxactivexcontrol/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetType](./gettype/) | Ottiene il tipo del controllo ActiveX. |
| [GetBorderStyle](./getborderstyle/) | Ottiene e imposta il tipo di bordo utilizzato dal controllo. |
| [SetBorderStyle](./setborderstyle/) | Ottiene e imposta il tipo di bordo utilizzato dal controllo. |
| [GetBorderOleColor](./getborderolecolor/) | Ottiene e imposta il colore OLE dello sfondo. |
| [SetBorderOleColor](./setborderolecolor/) | Ottiene e imposta il colore OLE dello sfondo. |
| [GetSpecialEffect](./getspecialeffect/) | Ottiene e imposta l'effetto speciale del controllo. |
| [SetSpecialEffect](./setspecialeffect/) | Ottiene e imposta l'effetto speciale del controllo. |
| [GetMaxLength](./getmaxlength/) | Ottiene e imposta il numero massimo di caratteri |
| [SetMaxLength](./setmaxlength/) | Ottiene e imposta il numero massimo di caratteri |
| [GetScrollBars](./getscrollbars/) | Indica se il controllo ha barre di scorrimento verticali, orizzontali, entrambe o nessuna. |
| [SetScrollBars](./setscrollbars/) | Indica se il controllo ha barre di scorrimento verticali, orizzontali, entrambe o nessuna. |
| [GetPasswordChar](./getpasswordchar/) | Ottiene e imposta un carattere da visualizzare al posto dei caratteri inseriti. |
| [SetPasswordChar](./setpasswordchar/) | Ottiene e imposta un carattere da visualizzare al posto dei caratteri inseriti. |
| [IsEditable](./iseditable/) | Indica se l'utente può digitare nel controllo. |
| [SetIsEditable](./setiseditable/) | Indica se l'utente può digitare nel controllo. |
| [GetIntegralHeight](./getintegralheight/) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [SetIntegralHeight](./setintegralheight/) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [IsDragBehaviorEnabled](./isdragbehaviorenabled/) | Indica se il trascinamento e il rilascio sono abilitati per il controllo. |
| [SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | Indica se il trascinamento e il rilascio sono abilitati per il controllo. |
| [GetEnterKeyBehavior](./getenterkeybehavior/) | Specifica il comportamento del tasto ENTER.True specifica che premere ENTER creerà una nuova riga.False specifica che premere ENTER sposterà il focus al prossimo oggetto nell'ordine di tabulazione. |
| [SetEnterKeyBehavior](./setenterkeybehavior/) | Specifica il comportamento del tasto ENTER.True specifica che premere ENTER creerà una nuova riga.False specifica che premere ENTER sposterà il focus al prossimo oggetto nell'ordine di tabulazione. |
| [GetEnterFieldBehavior](./getenterfieldbehavior/) | Specifica il comportamento della selezione quando si entra nel controllo. True specifica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False specifica che tutto il testo nel controllo sarà selezionato quando si entra nel controllo. |
| [SetEnterFieldBehavior](./setenterfieldbehavior/) | Specifica il comportamento della selezione quando si entra nel controllo. True specifica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False specifica che tutto il testo nel controllo sarà selezionato quando si entra nel controllo. |
| [GetTabKeyBehavior](./gettabkeybehavior/) | Indica se i caratteri di tabulazione sono consentiti nel testo del controllo. |
| [SetTabKeyBehavior](./settabkeybehavior/) | Indica se i caratteri di tabulazione sono consentiti nel testo del controllo. |
| [GetHideSelection](./gethideselection/) | Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il focus. |
| [SetHideSelection](./sethideselection/) | Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il focus. |
| [IsAutoTab](./isautotab/) | Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri. |
| [SetIsAutoTab](./setisautotab/) | Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri. |
| [IsMultiLine](./ismultiline/) | Indica se il controllo può visualizzare più di una riga di testo. |
| [SetIsMultiLine](./setismultiline/) | Indica se il controllo può visualizzare più di una riga di testo. |
| [IsWordWrapped](./iswordwrapped/) | Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga. |
| [SetIsWordWrapped](./setiswordwrapped/) | Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga. |
| [GetText](./gettext/) | Ottiene e imposta il testo del controllo. |
| [SetText](./settext/) | Ottiene e imposta il testo del controllo. |
| [GetDropButtonStyle](./getdropbuttonstyle/) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [SetDropButtonStyle](./setdropbuttonstyle/) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [IsAutoWordSelected](./isautowordselected/) | Specifica l'unità base utilizzata per estendere una selezione. True specifica che l'unità base è un singolo carattere. false specifica che l'unità base è una parola intera. |
| [SetIsAutoWordSelected](./setisautowordselected/) | Specifica l'unità base utilizzata per estendere una selezione. True specifica che l'unità base è un singolo carattere. false specifica che l'unità base è una parola intera. |
| [IsEnabled](./isenabled/) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [SetIsEnabled](./setisenabled/) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [IsLocked](./islocked/) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [SetIsLocked](./setislocked/) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [IsTransparent](./istransparent/) | Indica se il controllo è trasparente. |
| [SetIsTransparent](./setistransparent/) | Indica se il controllo è trasparente. |
| [GetIMEMode](./getimemode/) | Ottiene e imposta la modalità di esecuzione predefinita dell'Editor di Metodo di Input per il controllo quando riceve il focus. |
| [SetIMEMode](./setimemode/) | Ottiene e imposta la modalità di esecuzione predefinita dell'Editor di Metodo di Input per il controllo quando riceve il focus. |
| [GetFont](./getfont/) | Rappresenta il carattere del controllo. |
| [GetTextAlign](./gettextalign/) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [SetTextAlign](./settextalign/) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [GetData](./getdata/) | Ottiene e imposta i dati binari del controllo. |
| [IsAutoSize](./isautosize/) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [SetIsAutoSize](./setisautosize/) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [GetWorkbook](./getworkbook/) | Ottiene l'oggetto Workbook. |
| [GetMouseIcon](./getmouseicon/) | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [SetMouseIcon](./setmouseicon/) | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [GetMousePointer](./getmousepointer/) | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [SetMousePointer](./setmousepointer/) | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [GetLinkedCell](./getlinkedcell/) | Ottiene e imposta la cella collegata. |
| [SetLinkedCell](./setlinkedcell/) | Ottiene e imposta la cella collegata. |
| [GetListFillRange](./getlistfillrange/) | Ottiene e imposta l'intervallo di riempimento dell'elenco. |
| [SetListFillRange](./setlistfillrange/) | Ottiene e imposta l'intervallo di riempimento dell'elenco. |
| [GetWidth](./getwidth/) | Ottiene e imposta la larghezza del controllo in unità di punti. |
| [SetWidth](./setwidth/) | Ottiene e imposta la larghezza del controllo in unità di punti. |
| [GetHeight](./getheight/) | Ottiene e imposta l'altezza del controllo in unità di punti. |
| [SetHeight](./setheight/) | Ottiene e imposta l'altezza del controllo in unità di punti. |
| [GetForeOleColor](./getforeolecolor/) | Ottiene e imposta il colore OLE del primo piano. |
| [SetForeOleColor](./setforeolecolor/) | Ottiene e imposta il colore OLE del primo piano. |
| [GetBackOleColor](./getbackolecolor/) | Ottiene e imposta il colore OLE dello sfondo. |
| [SetBackOleColor](./setbackolecolor/) | Ottiene e imposta il colore OLE dello sfondo. |
| [IsVisible](./isvisible/) | Indica se questo controllo è visibile. |
| [SetIsVisible](./setisvisible/) | Indica se questo controllo è visibile. |
| [GetShadow](./getshadow/) | Indica se mostrare un'ombra. |
| [SetShadow](./setshadow/) | Indica se mostrare un'ombra. |
