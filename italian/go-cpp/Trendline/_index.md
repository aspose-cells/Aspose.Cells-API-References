---
title: "Trendline Classe"
linktitle: "Trendline"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Trendline classe. Incapsula l'oggetto che rappresenta trendline in Go."
type: docs
weight: 200
url: /it/go-cpp/trendline/
---

## Trendline class

Rappresenta una linea di tendenza in un grafico.

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewTrendline](./newtrendline/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [IsNameAuto](./isnameauto/) | Restituisce se Microsoft Excel determina automaticamente il nome della trendline. |
| [SetIsNameAuto](./setisnameauto/) | Restituisce se Microsoft Excel determina automaticamente il nome della trendline. |
| [GetType](./gettype/) | Restituisce il tipo di trendline. |
| [GetName](./getname/) | Restituisce il nome della trendline. |
| [SetName](./setname/) | Restituisce il nome della trendline. |
| [GetOrder](./getorder/) | Restituisce o imposta l'ordine della trendline (un intero maggiore di 1) quando il tipo di trendline è Polinomiale. L'ordine deve essere compreso tra 2 e 6. |
| [SetOrder](./setorder/) | Restituisce o imposta l'ordine della trendline (un intero maggiore di 1) quando il tipo di trendline è Polinomiale. L'ordine deve essere compreso tra 2 e 6. |
| [GetPeriod](./getperiod/) | Restituisce o imposta il periodo per la trendline a media mobile. |
| [SetPeriod](./setperiod/) | Restituisce o imposta il periodo per la trendline a media mobile. |
| [GetForward](./getforward/) | Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) che la trendline si estende in avanti. Il numero di periodi deve essere maggiore o uguale a zero. |
| [SetForward](./setforward/) | Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) che la trendline si estende in avanti. Il numero di periodi deve essere maggiore o uguale a zero. |
| [GetBackward](./getbackward/) | Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) che la trendline si estende all'indietro. Il numero di periodi deve essere maggiore o uguale a zero. Se il tipo di grafico è colonna, il numero di periodi deve essere compreso tra 0 e 0,5. |
| [SetBackward](./setbackward/) | Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) che la trendline si estende all'indietro. Il numero di periodi deve essere maggiore o uguale a zero. Se il tipo di grafico è colonna, il numero di periodi deve essere compreso tra 0 e 0,5. |
| [GetDisplayEquation](./getdisplayequation/) | Rappresenta se l'equazione della trendline è visualizzata sul grafico (nella stessa etichetta dati del valore R-quadrato). Impostare questa proprietà su True attiva automaticamente le etichette dati. |
| [SetDisplayEquation](./setdisplayequation/) | Rappresenta se l'equazione della trendline è visualizzata sul grafico (nella stessa etichetta dati del valore R-quadrato). Impostare questa proprietà su True attiva automaticamente le etichette dati. |
| [GetDisplayRSquared](./getdisplayrsquared/) | Rappresenta se il valore R-quadrato della trendline è visualizzato sul grafico (nella stessa etichetta dati dell'equazione). Impostare questa proprietà su True attiva automaticamente le etichette dati. |
| [SetDisplayRSquared](./setdisplayrsquared/) | Rappresenta se il valore R-quadrato della trendline è visualizzato sul grafico (nella stessa etichetta dati dell'equazione). Impostare questa proprietà su True attiva automaticamente le etichette dati. |
| [GetIntercept](./getintercept/) | Restituisce o imposta il punto in cui la trendline attraversa l'asse dei valori. |
| [SetIntercept](./setintercept/) | Restituisce o imposta il punto in cui la trendline attraversa l'asse dei valori. |
| [GetDataLabels](./getdatalabels/) | Rappresenta l'oggetto DataLabels per la serie specificata. |
| [GetLegendEntry](./getlegendentry/) | Ottiene la voce della legenda corrispondente a questa trendline. |
| [GetCompoundType](./getcompoundtype/) | Specifica il tipo di linea composta |
| [SetCompoundType](./setcompoundtype/) | Specifica il tipo di linea composta |
| [GetDashType](./getdashtype/) | Specifica il tipo di linea tratteggiata |
| [SetDashType](./setdashtype/) | Specifica il tipo di linea tratteggiata |
| [GetCapType](./getcaptype/) | Specifica le estremità finali. |
| [SetCapType](./setcaptype/) | Specifica le estremità finali. |
| [GetJoinType](./getjointype/) | Specifica le estremità di giunzione. |
| [SetJoinType](./setjointype/) | Specifica le estremità di giunzione. |
| [GetBeginType](./getbegintype/) | Specifica una punta di freccia per l'inizio di una linea. |
| [SetBeginType](./setbegintype/) | Specifica una punta di freccia per l'inizio di una linea. |
| [GetEndType](./getendtype/) | Specifica una punta di freccia per la fine di una linea. |
| [SetEndType](./setendtype/) | Specifica una punta di freccia per la fine di una linea. |
| [GetBeginArrowLength](./getbeginarrowlength/) | Specifica la lunghezza della punta di freccia per l'inizio di una linea. |
| [SetBeginArrowLength](./setbeginarrowlength/) | Specifica la lunghezza della punta di freccia per l'inizio di una linea. |
| [GetEndArrowLength](./getendarrowlength/) | Specifica la lunghezza della punta di freccia per la fine di una linea. |
| [SetEndArrowLength](./setendarrowlength/) | Specifica la lunghezza della punta di freccia per la fine di una linea. |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | Specifica la larghezza della punta di freccia per l'inizio di una linea. |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | Specifica la larghezza della punta di freccia per l'inizio di una linea. |
| [GetEndArrowWidth](./getendarrowwidth/) | Specifica la larghezza della punta di freccia per la fine di una linea. |
| [SetEndArrowWidth](./setendarrowwidth/) | Specifica la larghezza della punta di freccia per la fine di una linea. |
| [GetThemeColor](./getthemecolor/) | Ottiene e imposta il colore del tema. |
| [SetThemeColor](./setthemecolor/) | Ottiene e imposta il colore del tema. |
| [GetColor](./getcolor/) | Rappresenta il colore della linea. |
| [SetColor](./setcolor/) | Rappresenta il colore della linea. |
| [GetTransparency](./gettransparency/) | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (chiaro). |
| [SetTransparency](./settransparency/) | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (chiaro). |
| [GetStyle](./getstyle/) | Rappresenta lo stile della linea. |
| [SetStyle](./setstyle/) | Rappresenta lo stile della linea. |
| [GetWeight](./getweight/) | Ottiene o imposta il WeightType della linea. |
| [SetWeight](./setweight/) | Ottiene o imposta il WeightType della linea. |
| [GetWeightPt](./getweightpt/) | Ottiene o imposta il peso della linea in unità di punti. |
| [SetWeightPt](./setweightpt/) | Ottiene o imposta il peso della linea in unità di punti. |
| [GetWeightPx](./getweightpx/) | Ottiene o imposta il peso della linea in unità di pixel. |
| [SetWeightPx](./setweightpx/) | Ottiene o imposta il peso della linea in unità di pixel. |
| [GetFormattingType](./getformattingtype/) | Ottiene o imposta il tipo di formato. |
| [SetFormattingType](./setformattingtype/) | Ottiene o imposta il tipo di formato. |
| [IsAutomaticColor](./isautomaticcolor/) | Indica se il colore della linea è assegnato automaticamente. |
| [IsVisible](./isvisible/) | Rappresenta se la linea è visibile. |
| [SetIsVisible](./setisvisible/) | Rappresenta se la linea è visibile. |
| [IsAuto](./isauto/) | Indica se questo stile di linea è assegnato automaticamente. |
| [SetIsAuto](./setisauto/) | Indica se questo stile di linea è assegnato automaticamente. |
| [GetGradientFill](./getgradientfill/) | Rappresenta il riempimento gradiente. |
