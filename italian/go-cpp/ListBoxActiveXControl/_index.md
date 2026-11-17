---
title: "Classe ListBoxActiveXControl"
linktitle: "ListBoxActiveXControl"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ListBoxActiveXControl. Incapsula l'oggetto che rappresenta listboxactivexcontrol in Go."
type: docs
weight: 200
url: /it/go-cpp/listboxactivexcontrol/
---

## ListBoxActiveXControl class

Rappresenta un controllo ActiveX ListBox.

```go

type ListBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewListBoxActiveXControl](./newlistboxactivexcontrol/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetType](./gettype/) | Ottiene il tipo del controllo ActiveX. |
| [GetScrollBars](./getscrollbars/) | Indica se il controllo ha barre di scorrimento verticali, orizzontali, entrambe o nessuna. |
| [SetScrollBars](./setscrollbars/) | Indica se il controllo ha barre di scorrimento verticali, orizzontali, entrambe o nessuna. |
| [GetListWidth](./getlistwidth/) | Ottiene e imposta la larghezza in unità di punti. |
| [SetListWidth](./setlistwidth/) | Ottiene e imposta la larghezza in unità di punti. |
| [GetBoundColumn](./getboundcolumn/) | Rappresenta come la proprietà Value è determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect (fmMultiSelectSingle). |
| [SetBoundColumn](./setboundcolumn/) | Rappresenta come la proprietà Value è determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect (fmMultiSelectSingle). |
| [GetTextColumn](./gettextcolumn/) | Rappresenta la colonna in un ComboBox o ListBox da visualizzare all'utente. |
| [SetTextColumn](./settextcolumn/) | Rappresenta la colonna in un ComboBox o ListBox da visualizzare all'utente. |
| [GetColumnCount](./getcolumncount/) | Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox. |
| [SetColumnCount](./setcolumncount/) | Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox. |
| [GetMatchEntry](./getmatchentry/) | Indica come un ListBox o ComboBox ricerca la sua lista mentre l'utente digita. |
| [SetMatchEntry](./setmatchentry/) | Indica come un ListBox o ComboBox ricerca la sua lista mentre l'utente digita. |
| [GetListStyle](./getliststyle/) | Ottiene e imposta l'aspetto visivo. |
| [SetListStyle](./setliststyle/) | Ottiene e imposta l'aspetto visivo. |
| [GetSelectionType](./getselectiontype/) | Indica se il controllo consente selezioni multiple. |
| [SetSelectionType](./setselectiontype/) | Indica se il controllo consente selezioni multiple. |
| [GetValue](./getvalue/) | Ottiene e imposta il valore del controllo. |
| [SetValue](./setvalue/) | Ottiene e imposta il valore del controllo. |
| [GetBorderStyle](./getborderstyle/) | Ottiene e imposta il tipo di bordo utilizzato dal controllo. |
| [SetBorderStyle](./setborderstyle/) | Ottiene e imposta il tipo di bordo utilizzato dal controllo. |
| [GetBorderOleColor](./getborderolecolor/) | Ottiene e imposta il colore OLE dello sfondo. |
| [SetBorderOleColor](./setborderolecolor/) | Ottiene e imposta il colore OLE dello sfondo. |
| [GetSpecialEffect](./getspecialeffect/) | Ottiene e imposta l'effetto speciale del controllo. |
| [SetSpecialEffect](./setspecialeffect/) | Ottiene e imposta l'effetto speciale del controllo. |
| [GetShowColumnHeads](./getshowcolumnheads/) | Indica se le intestazioni di colonna sono visualizzate. |
| [SetShowColumnHeads](./setshowcolumnheads/) | Indica se le intestazioni di colonna sono visualizzate. |
| [GetIntegralHeight](./getintegralheight/) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [SetIntegralHeight](./setintegralheight/) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [GetColumnWidths](./getcolumnwidths/) | Ottiene e imposta la larghezza della colonna. |
| [SetColumnWidths](./setcolumnwidths/) | Ottiene e imposta la larghezza della colonna. |
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
