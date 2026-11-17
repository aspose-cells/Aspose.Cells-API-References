---
title: "Series classe"
linktitle: "Series"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Series classe. Incapsula l'oggetto che rappresenta series in Go."
type: docs
weight: 200
url: /it/go-cpp/series/
---

## Series class

Incapsula l'oggetto che rappresenta una singola serie di dati in un grafico.

```go

type Series struct  {
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
| [IsFiltered](./isfiltered/) | Indica se la serie è selezionata o filtrata. True indica che questa serie è filtrata e non verrà visualizzata nel grafico. |
| [SetIsFiltered](./setisfiltered/) | Indica se la serie è selezionata o filtrata. True indica che questa serie è filtrata e non verrà visualizzata nel grafico. |
| [GetLayoutProperties](./getlayoutproperties/) | Rappresenta le proprietà del layout. |
| [Move](./move/) | Sposta la serie su o giù. |
| [GetPoints](./getpoints/) | Ottiene la collezione di punti in una serie in un grafico. |
| [GetArea](./getarea/) | Rappresenta l'area di sfondo dell'oggetto Series. |
| [GetBorder](./getborder/) | Rappresenta il bordo di un oggetto Series. |
| [GetName](./getname/) | Ottiene o imposta il nome della serie di dati. |
| [SetName](./setname/) | Ottiene o imposta il nome della serie di dati. |
| [GetDisplayName](./getdisplayname/) | Ottiene il nome della serie che viene visualizzato sul grafico. |
| [GetCountOfDataValues](./getcountofdatavalues/) | Ottiene il numero dei valori dei dati. |
| [IsVerticalValues](./isverticalvalues/) | Indica se l'origine dati è verticale. |
| [GetValues](./getvalues/) | Rappresenta i valori Y di questa serie di grafico. |
| [SetValues](./setvalues/) | Rappresenta i valori Y di questa serie di grafico. |
| [GetPointValues](./getpointvalues/) | Ottiene i valori effettivi che vengono usati per tracciare ogni punto di questa serie nel grafico. |
| [GetCategoryValues](./getcategoryvalues/) | Ottiene i valori di categoria effettivi che vengono usati per tracciare ogni punto di questa serie nel grafico. |
| [GetValuesFormatCode](./getvaluesformatcode/) | Rappresenta il codice di formato della NumberList dei Valori. |
| [SetValuesFormatCode](./setvaluesformatcode/) | Rappresenta il codice di formato della NumberList dei Valori. |
| [GetXValuesFormatCode](./getxvaluesformatcode/) | Rappresenta il codice di formato della NumberList dei Valori X. |
| [SetXValuesFormatCode](./setxvaluesformatcode/) | Rappresenta il codice di formato della NumberList dei Valori X. |
| [GetXValues](./getxvalues/) | Rappresenta i valori X di questa serie di grafico. |
| [SetXValues](./setxvalues/) | Rappresenta i valori X di questa serie di grafico. |
| [GetBubbleSizes](./getbubblesizes/) | Ottiene o imposta i valori di dimensione delle bolle della serie di grafico. |
| [SetBubbleSizes](./setbubblesizes/) | Ottiene o imposta i valori di dimensione delle bolle della serie di grafico. |
| [GetTrendLines](./gettrendlines/) | Restituisce tutte le linee di tendenza di questa serie. |
| [GetSmooth](./getsmooth/) | Rappresenta l'ammorbidimento della curva. True se l'ammorbidimento è attivato per il grafico a linee o a dispersione. Si applica solo ai grafici a linee e ai grafici a dispersione con linee. |
| [SetSmooth](./setsmooth/) | Rappresenta l'ammorbidimento della curva. True se l'ammorbidimento è attivato per il grafico a linee o a dispersione. Si applica solo ai grafici a linee e ai grafici a dispersione con linee. |
| [GetShadow](./getshadow/) | True se la serie ha un'ombra. |
| [SetShadow](./setshadow/) | True se la serie ha un'ombra. |
| [GetHas3DEffect](./gethas3deffect/) | True se la serie ha un aspetto tridimensionale. |
| [SetHas3DEffect](./sethas3deffect/) | True se la serie ha un aspetto tridimensionale. |
| [GetBar3DShapeType](./getbar3dshapetype/) | Ottiene o imposta il tipo di forma 3D usato con il grafico a barre o colonne 3-D. |
| [SetBar3DShapeType](./setbar3dshapetype/) | Ottiene o imposta il tipo di forma 3D usato con il grafico a barre o colonne 3-D. |
| [GetDataLabels](./getdatalabels/) | Rappresenta l'oggetto DataLabels per l'ASeries specificato. |
| [GetType](./gettype/) | Ottiene o imposta il tipo di una serie di dati. |
| [SetType](./settype/) | Ottiene o imposta il tipo di una serie di dati. |
| [GetMarker](./getmarker/) | Ottiene il Marker</see>. |
| [GetPlotOnSecondAxis](./getplotonsecondaxis/) | Indica se questa serie è tracciata sul secondo asse dei valori. |
| [SetPlotOnSecondAxis](./setplotonsecondaxis/) | Indica se questa serie è tracciata sul secondo asse dei valori. |
| [GetXErrorBar](./getxerrorbar/) | Rappresenta la barra di errore in direzione X della serie. |
| [GetYErrorBar](./getyerrorbar/) | Rappresenta la barra di errore in direzione Y della serie. |
| [GetHasHiLoLines](./gethashilolines/) | True se il grafico a linee ha linee alto-basso. Si applica solo ai grafici a linee. |
| [SetHasHiLoLines](./sethashilolines/) | True se il grafico a linee ha linee alto-basso. Si applica solo ai grafici a linee. |
| [GetHiLoLines](./gethilolines/) | Restituisce un oggetto HiLoLines che rappresenta le linee alto-basso per una serie su un grafico a linee. Si applica solo ai grafici a linee. |
| [GetHasSeriesLines](./gethasserieslines/) | Vero se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. Si applica solo a grafici a colonne impilate, a barre, Pie of Pie o Bar of Pie. |
| [SetHasSeriesLines](./sethasserieslines/) | Vero se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. Si applica solo a grafici a colonne impilate, a barre, Pie of Pie o Bar of Pie. |
| [GetSeriesLines](./getserieslines/) | Restituisce un oggetto SeriesLines che rappresenta le linee di serie per un grafico a barre impilate o a colonne impilate. Si applica solo a grafici a barre impilate e a colonne impilate. |
| [GetHasDropLines](./gethasdroplines/) | Vero se il grafico ha linee di discesa. Si applica solo a grafici a linee o a aree. |
| [SetHasDropLines](./sethasdroplines/) | Vero se il grafico ha linee di discesa. Si applica solo a grafici a linee o a aree. |
| [GetDropLines](./getdroplines/) | Restituisce un oggetto Line che rappresenta le linee di discesa per una serie nel grafico a linee o a aree. Si applica solo a grafici a linee o a aree. |
| [GetHasUpDownBars](./gethasupdownbars/) | Vero se un grafico a linee ha barre su e giù. Si applica solo a grafici a linee. |
| [SetHasUpDownBars](./sethasupdownbars/) | Vero se un grafico a linee ha barre su e giù. Si applica solo a grafici a linee. |
| [GetUpBars](./getupbars/) | Restituisce un oggetto DropBars che rappresenta le barre su in un grafico a linee. Si applica solo a grafici a linee. |
| [GetDownBars](./getdownbars/) | Restituisce un oggetto DropBars che rappresenta le barre giù in un grafico a linee. Si applica solo a grafici a linee. |
| [IsColorVaried](./iscolorvaried/) | Rappresenta se il colore dei punti è variabile. Il grafico deve contenere una sola serie o essere un grafico a torta. |
| [SetIsColorVaried](./setiscolorvaried/) | Rappresenta se il colore dei punti è variabile. Il grafico deve contenere una sola serie o essere un grafico a torta. |
| [GetGapWidth](./getgapwidth/) | Restituisce o imposta lo spazio tra i gruppi di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [SetGapWidth](./setgapwidth/) | Restituisce o imposta lo spazio tra i gruppi di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Ottiene o imposta l'angolo della prima fetta di grafico a torta o a ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3D e a ciambella, con valori da 0 a 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Ottiene o imposta l'angolo della prima fetta di grafico a torta o a ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3D e a ciambella, con valori da 0 a 360. |
| [GetOverlap](./getoverlap/) | Specifica come sono posizionate le barre e le colonne. Può essere un valore compreso tra -100 e 100. Si applica solo a grafici a barre 2D e a colonne 2D. |
| [SetOverlap](./setoverlap/) | Specifica come sono posizionate le barre e le colonne. Può essere un valore compreso tra -100 e 100. Si applica solo a grafici a barre 2D e a colonne 2D. |
| [GetSecondPlotSize](./getsecondplotsize/) | Restituisce o imposta la dimensione della sezione secondaria di un grafico Pie of Pie o Bar of Pie, come percentuale della dimensione della torta primaria. Può essere un valore da 5 a 200. |
| [SetSecondPlotSize](./setsecondplotsize/) | Restituisce o imposta la dimensione della sezione secondaria di un grafico Pie of Pie o Bar of Pie, come percentuale della dimensione della torta primaria. Può essere un valore da 5 a 200. |
| [GetSplitType](./getsplittype/) | Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico Pie of Pie o Bar of Pie. |
| [SetSplitType](./setsplittype/) | Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico Pie of Pie o Bar of Pie. |
| [GetSplitValue](./getsplitvalue/) | Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda torta o barra in un grafico Pie of Pie o Bar of Pie. |
| [SetSplitValue](./setsplitvalue/) | Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda torta o barra in un grafico Pie of Pie o Bar of Pie. |
| [IsAutoSplit](./isautosplit/) | Indica se il valore soglia è automatico. |
| [GetBubbleScale](./getbubblescale/) | Ottiene o imposta il fattore di scala per le bolle nel gruppo di grafico specificato. Può essere un valore intero da 0 (zero) a 300, corrispondente a una percentuale della dimensione predefinita. Si applica solo a grafici a bolle. |
| [SetBubbleScale](./setbubblescale/) | Ottiene o imposta il fattore di scala per le bolle nel gruppo di grafico specificato. Può essere un valore intero da 0 (zero) a 300, corrispondente a una percentuale della dimensione predefinita. Si applica solo a grafici a bolle. |
| [GetSizeRepresents](./getsizerepresents/) | Ottiene o imposta cosa rappresenta la dimensione della bolla in un grafico a bolle. |
| [SetSizeRepresents](./setsizerepresents/) | Ottiene o imposta cosa rappresenta la dimensione della bolla in un grafico a bolle. |
| [GetShowNegativeBubbles](./getshownegativebubbles/) | Vero se le bolle negative sono visualizzate per il gruppo di grafico. Valido solo per grafici a bolle. |
| [SetShowNegativeBubbles](./setshownegativebubbles/) | Vero se le bolle negative sono visualizzate per il gruppo di grafico. Valido solo per grafici a bolle. |
| [GetDoughnutHoleSize](./getdoughnutholesize/) | Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. La dimensione del foro è espressa come percentuale della dimensione del grafico, tra il 10% e il 90%. |
| [SetDoughnutHoleSize](./setdoughnutholesize/) | Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. La dimensione del foro è espressa come percentuale della dimensione del grafico, tra il 10% e il 90%. |
| [GetExplosion](./getexplosion/) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [SetExplosion](./setexplosion/) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [GetHasRadarAxisLabels](./gethasradaraxislabels/) | Vero se un grafico radar ha etichette dell'asse di categoria. Si applica solo a grafici radar. |
| [SetHasRadarAxisLabels](./sethasradaraxislabels/) | Vero se un grafico radar ha etichette dell'asse di categoria. Si applica solo a grafici radar. |
| [GetHasLeaderLines](./gethasleaderlines/) | Vero se la serie ha linee guida. |
| [SetHasLeaderLines](./sethasleaderlines/) | Vero se la serie ha linee guida. |
| [GetLeaderLines](./getleaderlines/) | Rappresenta le linee guida su un grafico. Le linee guida collegano le etichette dei dati ai punti dati. Questo oggetto non è una collezione; non esiste un oggetto che rappresenti una singola linea guida. |
| [GetLegendEntry](./getlegendentry/) | Ottiene la voce della legenda corrispondente a questa serie. |
| [GetShapeProperties](./getshapeproperties/) | Ottiene l'oggetto ShapePropertyCollection che contiene le proprietà visive della forma della Serie. |
