---
title: "Classe Style"
linktitle: "Style"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Style. Incapsula l'oggetto che rappresenta style in Go."
type: docs
weight: 200
url: /it/go-cpp/style/
---

## Style class

Rappresenta lo stile di visualizzazione del documento Excel, come carattere, colore, allineamento, bordo, ecc. L'oggetto Style contiene tutti gli attributi di stile (carattere, formato numerico, allineamento e così via) come proprietà.

```go

type Style struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | Ottiene e imposta il colore del tema di sfondo. |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | Ottiene e imposta il colore del tema di sfondo. |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | Ottiene e imposta il colore del tema di primo piano. |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | Ottiene e imposta il colore del tema di primo piano. |
| [GetName](./getname/) | Ottiene o imposta il nome dello stile. |
| [SetName](./setname/) | Ottiene o imposta il nome dello stile. |
| [GetPattern](./getpattern/) | Ottiene o imposta il tipo di motivo di sfondo della cella. |
| [SetPattern](./setpattern/) | Ottiene o imposta il tipo di motivo di sfondo della cella. |
| [SetPatternColor](./setpatterncolor/) | Imposta il colore di sfondo. |
| [GetBorders](./getborders/) | Ottiene la BorderCollection dello stile. |
| [GetBackgroundColor](./getbackgroundcolor/) | Ottiene o imposta il colore di sfondo di uno stile. |
| [SetBackgroundColor](./setbackgroundcolor/) | Ottiene o imposta il colore di sfondo di uno stile. |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | Ottiene e imposta il colore di sfondo con un valore ARGB a 32 bit. |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | Ottiene e imposta il colore di sfondo con un valore ARGB a 32 bit. |
| [GetForegroundColor](./getforegroundcolor/) | Ottiene o imposta il colore di primo piano di uno stile. |
| [SetForegroundColor](./setforegroundcolor/) | Ottiene o imposta il colore di primo piano di uno stile. |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | Ottiene e imposta il colore di primo piano con un valore ARGB a 32 bit. |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | Ottiene e imposta il colore di primo piano con un valore ARGB a 32 bit. |
| [Copy](./copy/) | Copia i dati da un altro oggetto stile |
| [GetHasBorders](./gethasborders/) | Verifica se sono stati impostati bordi per lo stile. |
| [GetParentStyle](./getparentstyle/) | Ottiene lo stile genitore di questo stile. |
| [Update](./update/) | Applica lo stile denominato agli stili delle celle che utilizzano questo stile denominato. Funziona come fare clic sul pulsante "ok" dopo aver terminato la modifica dello stile. Si applica solo agli stili denominati. |
| [IsNumberFormatApplied](./isnumberformatapplied/) | Indica se la formattazione numerica deve essere applicata. |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | Indica se la formattazione numerica deve essere applicata. |
| [IsFontApplied](./isfontapplied/) | Indica se la formattazione del carattere deve essere applicata. |
| [SetIsFontApplied](./setisfontapplied/) | Indica se la formattazione del carattere deve essere applicata. |
| [IsAlignmentApplied](./isalignmentapplied/) | Indica se la formattazione dell'allineamento deve essere applicata. |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | Indica se la formattazione dell'allineamento deve essere applicata. |
| [IsBorderApplied](./isborderapplied/) | Indica se la formattazione del bordo deve essere applicata. |
| [SetIsBorderApplied](./setisborderapplied/) | Indica se la formattazione del bordo deve essere applicata. |
| [IsFillApplied](./isfillapplied/) | Indica se la formattazione di riempimento deve essere applicata. |
| [SetIsFillApplied](./setisfillapplied/) | Indica se la formattazione di riempimento deve essere applicata. |
| [IsProtectionApplied](./isprotectionapplied/) | Indica se la formattazione di protezione deve essere applicata. |
| [SetIsProtectionApplied](./setisprotectionapplied/) | Indica se la formattazione di protezione deve essere applicata. |
| [IsModified](./ismodified/) | Verifica se le proprietà specificate dello stile sono state modificate. Utilizzato per lo stile di ConditionalFormattings per verificare se le proprietà specificate di questo stile devono essere usate durante l'applicazione di ConditionalFormattings su una cella. |
| [Equals](./equals/) | Determina se due istanze di Style sono uguali. |
| [GetHashCode](./gethashcode/) | Funziona come funzione hash per un oggetto Style. |
| [GetIndentLevel](./getindentlevel/) | Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un intero da 0 a 250. |
| [SetIndentLevel](./setindentlevel/) | Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un intero da 0 a 250. |
| [GetFont](./getfont/) | Ottiene un oggetto Font. |
| [GetRotationAngle](./getrotationangle/) | Rappresenta l'angolo di rotazione del testo. |
| [SetRotationAngle](./setrotationangle/) | Rappresenta l'angolo di rotazione del testo. |
| [GetHorizontalAlignment](./gethorizontalalignment/) | Ottiene o imposta il tipo di allineamento orizzontale del testo in una cella. |
| [SetHorizontalAlignment](./sethorizontalalignment/) | Ottiene o imposta il tipo di allineamento orizzontale del testo in una cella. |
| [GetVerticalAlignment](./getverticalalignment/) | Ottiene o imposta il tipo di allineamento verticale del testo in una cella. |
| [SetVerticalAlignment](./setverticalalignment/) | Ottiene o imposta il tipo di allineamento verticale del testo in una cella. |
| [IsTextWrapped](./istextwrapped/) | Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo. |
| [SetIsTextWrapped](./setistextwrapped/) | Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo. |
| [GetNumber](./getnumber/) | Ottiene o imposta il formato di visualizzazione di numeri e date. I modelli di formattazione sono diversi per le varie regioni. |
| [SetNumber](./setnumber/) | Ottiene o imposta il formato di visualizzazione di numeri e date. I modelli di formattazione sono diversi per le varie regioni. |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | Imposta i bordi dello stile. |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | Imposta i bordi dello stile. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Imposta i bordi di contorno |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Imposta i bordi di contorno |
| [IsLocked](./islocked/) | Ottiene o imposta un valore che indica se una cella può essere modificata o meno. |
| [SetIsLocked](./setislocked/) | Ottiene o imposta un valore che indica se una cella può essere modificata o meno. |
| [SetCustom_String_Bool](./setcustom_string_bool/) | Imposta la stringa di formato numerico personalizzato di una cella. |
| [GetCustom](./getcustom/) | Rappresenta la stringa di formato numerico personalizzato di questo oggetto stile. Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), "" verrà restituito. |
| [SetCustom_String](./setcustom_string/) | Rappresenta la stringa di formato numerico personalizzato di questo oggetto stile. Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), "" verrà restituito. |
| [GetCultureCustom](./getculturecustom/) | Ottiene e imposta la stringa di modello dipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato. |
| [SetCultureCustom](./setculturecustom/) | Ottiene e imposta la stringa di modello dipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato. |
| [GetInvariantCustom](./getinvariantcustom/) | Ottiene la stringa di modello indipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato. |
| [IsFormulaHidden](./isformulahidden/) | Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto. |
| [SetIsFormulaHidden](./setisformulahidden/) | Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto. |
| [GetShrinkToFit](./getshrinktofit/) | Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile. |
| [SetShrinkToFit](./setshrinktofit/) | Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile. |
| [GetTextDirection](./gettextdirection/) | Rappresenta l'ordine di lettura del testo. |
| [SetTextDirection](./settextdirection/) | Rappresenta l'ordine di lettura del testo. |
| [IsJustifyDistributed](./isjustifydistributed/) | Indica se l'allineamento giustificato o distribuito delle celle deve essere usato sull'ultima riga di testo. |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | Indica se l'allineamento giustificato o distribuito delle celle deve essere usato sull'ultima riga di testo. |
| [GetQuotePrefix](./getquoteprefix/) | Indica se il valore della cella inizia con un apice singolo. |
| [SetQuotePrefix](./setquoteprefix/) | Indica se il valore della cella inizia con un apice singolo. |
| [IsGradient](./isgradient/) | Indica se l'ombreggiatura della cella è un modello a gradiente. |
| [SetIsGradient](./setisgradient/) | Indica se l'ombreggiatura della cella è un modello a gradiente. |
| [SetTwoColorGradient](./settwocolorgradient/) | Imposta il riempimento specificato a un gradiente a due colori. |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | Ottieni l'impostazione del gradiente a due colori. |
| [IsPercent](./ispercent/) | Indica se il formato numerico è un formato percentuale. |
| [IsDateTime](./isdatetime/) | Indica se il formato numerico è un formato data. |
| [IsCheckBox](./ischeckbox/) | Indica se è uno stile di casella di controllo |
| [SetIsCheckBox](./setischeckbox/) | Indica se è uno stile di casella di controllo |
| [ToJson](./tojson/) | Converti lo stile in dati struct JSON. |
| [GetLeftBorder](./getleftborder/) | Ottiene il bordo sinistro. |
| [GetRightBorder](./getrightborder/) | Ottiene il bordo destro. |
| [GetTopBorder](./gettopborder/) | Ottiene il bordo superiore. |
| [GetBottomBorder](./getbottomborder/) | Ottiene il bordo inferiore. |
