---
title: "DataLabels Classe"
linktitle: "DataLabels"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "DataLabels classe. Incapsula l'oggetto che rappresenta datalabels in Go."
type: docs
weight: 200
url: /it/go-cpp/datalabels/
---

## DataLabels class

Incapsula una raccolta di tutti gli oggetti DataLabel per la Serie specificata.

```go

type DataLabels struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewDataLabels](./newdatalabels/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetBorder](./getborder/) | Ottiene il Line</see>. |
| [GetArea](./getarea/) | Ottiene l'Area</see>. |
| [IsAutoText](./isautotext/) | Indica che il testo è generato automaticamente. |
| [SetIsAutoText](./setisautotext/) | Indica che il testo è generato automaticamente. |
| [GetDirectionType](./getdirectiontype/) | Ottiene e imposta la direzione del testo. |
| [SetDirectionType](./setdirectiontype/) | Ottiene e imposta la direzione del testo. |
| [GetText](./gettext/) | Ottiene o imposta il testo dell'etichetta dei dati. |
| [SetText](./settext/) | Ottiene o imposta il testo dell'etichetta dei dati. |
| [IsTextWrapped](./istextwrapped/) | Ottiene o imposta un valore che indica se il testo è a capo. |
| [SetIsTextWrapped](./setistextwrapped/) | Ottiene o imposta un valore che indica se il testo è a capo. |
| [GetBackgroundMode](./getbackgroundmode/) | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| [SetBackgroundMode](./setbackgroundmode/) | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| [GetShowValue](./getshowvalue/) | Rappresenta il comportamento di visualizzazione dei valori delle etichette dati di un grafico specificato. True visualizza i valori. False per nasconderli. |
| [SetShowValue](./setshowvalue/) | Rappresenta il comportamento di visualizzazione dei valori delle etichette dati di un grafico specificato. True visualizza i valori. False per nasconderli. |
| [GetShowCellRange](./getshowcellrange/) | Indica se mostrare l'intervallo di celle come etichette dati. |
| [SetShowCellRange](./setshowcellrange/) | Indica se mostrare l'intervallo di celle come etichette dati. |
| [GetShowPercentage](./getshowpercentage/) | Rappresenta il comportamento di visualizzazione del valore percentuale delle etichette dati di un grafico specificato. True visualizza il valore percentuale. False per nasconderlo. |
| [SetShowPercentage](./setshowpercentage/) | Rappresenta il comportamento di visualizzazione del valore percentuale delle etichette dati di un grafico specificato. True visualizza il valore percentuale. False per nasconderlo. |
| [GetShowBubbleSize](./getshowbubblesize/) | Rappresenta il comportamento di visualizzazione del valore percentuale delle etichette dati di un grafico specificato.True visualizza il valore percentuale.False nasconde il valore percentuale. |
| [SetShowBubbleSize](./setshowbubblesize/) | Rappresenta il comportamento di visualizzazione del valore percentuale delle etichette dati di un grafico specificato.True visualizza il valore percentuale.False nasconde il valore percentuale. |
| [GetShowCategoryName](./getshowcategoryname/) | Rappresenta il comportamento di visualizzazione del nome della categoria delle etichette dati di un grafico specificato.True per visualizzare il nome della categoria per le etichette dati su un grafico. False per nasconderlo. |
| [SetShowCategoryName](./setshowcategoryname/) | Rappresenta il comportamento di visualizzazione del nome della categoria delle etichette dati di un grafico specificato.True per visualizzare il nome della categoria per le etichette dati su un grafico. False per nasconderlo. |
| [GetShowSeriesName](./getshowseriesname/) | Indica se il nome della serie viene visualizzato sulle etichette dati di un grafico.True per mostrare il nome della serie.False per nasconderlo. |
| [SetShowSeriesName](./setshowseriesname/) | Indica se il nome della serie viene visualizzato sulle etichette dati di un grafico.True per mostrare il nome della serie.False per nasconderlo. |
| [GetShowLegendKey](./getshowlegendkey/) | Rappresenta il comportamento di visualizzazione della chiave della legenda delle etichette dati di un grafico specificato.True se la chiave della legenda delle etichette dati è visibile. |
| [SetShowLegendKey](./setshowlegendkey/) | Rappresenta il comportamento di visualizzazione della chiave della legenda delle etichette dati di un grafico specificato.True se la chiave della legenda delle etichette dati è visibile. |
| [Get_NumberFormat](./get_numberformat/) | Rappresenta la stringa di formato per l'oggetto DataLabels. |
| [SetNumberFormat](./setnumberformat/) | Rappresenta la stringa di formato per l'oggetto DataLabels. |
| [GetNumber](./getnumber/) | Ottiene e imposta il formato numerico predefinito. |
| [SetNumber](./setnumber/) | Ottiene e imposta il formato numerico predefinito. |
| [GetNumberFormatLinked](./getnumberformatlinked/) | Vero se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle). |
| [SetNumberFormatLinked](./setnumberformatlinked/) | Vero se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle). |
| [ApplyFont](./applyfont/) | Applica il carattere delle etichette dati a tutti i nodi figlio. |
| [GetFont](./getfont/) | Ottiene il carattere delle DataLabels; |
| [GetSeparatorType](./getseparatortype/) | Ottiene o imposta il tipo di separatore usato per le etichette dati su un grafico. |
| [SetSeparatorType](./setseparatortype/) | Ottiene o imposta il tipo di separatore usato per le etichette dati su un grafico. |
| [GetSeparatorValue](./getseparatorvalue/) | Ottiene o imposta il valore del separatore utilizzato per le etichette dei dati su un grafico. |
| [SetSeparatorValue](./setseparatorvalue/) | Ottiene o imposta il valore del separatore utilizzato per le etichette dei dati su un grafico. |
| [GetPosition](./getposition/) | Rappresenta la posizione dell'etichetta dei dati. |
| [SetPosition](./setposition/) | Rappresenta la posizione dell'etichetta dei dati. |
| [IsNeverOverlap](./isneveroverlap/) | Indica se le Datalabels non si sovrappongono mai durante la conversione di un Pie Chart in immagine. Nota: questa proprietà ha senso solo quando si converte un Pie Chart in immagine. |
| [SetIsNeverOverlap](./setisneveroverlap/) | Indica se le Datalabels non si sovrappongono mai durante la conversione di un Pie Chart in immagine. Nota: questa proprietà ha senso solo quando si converte un Pie Chart in immagine. |
| [GetShapeType](./getshapetype/) | Ottiene o imposta il tipo di forma dell'etichetta dei dati. |
| [SetShapeType](./setshapetype/) | Ottiene o imposta il tipo di forma dell'etichetta dei dati. |
| [IsInnerMode](./isinnermode/) | Indica se le dimensioni dell'area del grafico includono i segni di graduazione e le etichette degli assi. False specifica che le dimensioni devono determinare le dimensioni dell'area del grafico, dei segni di graduazione e delle etichette degli assi. |
| [SetIsInnerMode](./setisinnermode/) | Indica se le dimensioni dell'area del grafico includono i segni di graduazione e le etichette degli assi. False specifica che le dimensioni devono determinare le dimensioni dell'area del grafico, dei segni di graduazione e delle etichette degli assi. |
| [GetShadow](./getshadow/) | True se il frame ha un'ombra. |
| [SetShadow](./setshadow/) | True se il frame ha un'ombra. |
| [GetShapeProperties](./getshapeproperties/) | Ottiene l'oggetto ShapeProperties. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Rappresenta x della posizione predefinita in unità di Fraction dell'area del diagramma. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Rappresenta y della posizione predefinita in unità della frazione dell'area del diagramma. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Rappresenta la larghezza della posizione predefinita in unità di Fraction dell'area del diagramma. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Rappresenta l'altezza della posizione predefinita in unità della frazione dell'area del diagramma. |
| [GetTextOptions](./gettextoptions/) | Ottiene e imposta le opzioni del testo. |
| [GetAutoScaleFont](./getautoscalefont/) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True. |
| [SetAutoScaleFont](./setautoscalefont/) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True. |
| [IsAutomaticSize](./isautomaticsize/) | Indica se il frame del grafico è dimensionato automaticamente. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Indica se il frame del grafico è dimensionato automaticamente. |
| [GetXRatioToChart](./getxratiotochart/) | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. |
| [SetXRatioToChart](./setxratiotochart/) | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. |
| [GetYRatioToChart](./getyratiotochart/) | Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità del rapporto dell'area del grafico. |
| [SetYRatioToChart](./setyratiotochart/) | Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità del rapporto dell'area del grafico. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Ottiene o imposta la larghezza del frame in unità del rapporto dell'area del grafico. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Ottiene o imposta la larghezza del frame in unità del rapporto dell'area del grafico. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico. |
| [GetXPixel](./getxpixel/) | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di Pixel. |
| [SetXPixel](./setxpixel/) | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di Pixel. |
| [GetYPixel](./getypixel/) | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di pixel. |
| [SetYPixel](./setypixel/) | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di pixel. |
| [GetWidthPixel](./getwidthpixel/) | Ottiene o imposta la larghezza del frame in unità di Pixel. |
| [SetWidthPixel](./setwidthpixel/) | Ottiene o imposta la larghezza del frame in unità di Pixel. |
| [GetHeightPixel](./getheightpixel/) | Ottiene o imposta l'altezza del frame in unità di pixel. |
| [SetHeightPixel](./setheightpixel/) | Ottiene o imposta l'altezza del frame in unità di pixel. |
| [SetPositionAuto](./setpositionauto/) | Imposta la posizione del frame su automatico |
| [IsDeleted](./isdeleted/) | Indica se questa etichetta dati è eliminata. |
| [SetIsDeleted](./setisdeleted/) | Indica se questa etichetta dati è eliminata. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Ottiene e imposta l'allineamento orizzontale del testo. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Ottiene e imposta l'allineamento orizzontale del testo. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Ottiene o imposta l'allineamento verticale del testo. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Ottiene o imposta l'allineamento verticale del testo. |
| [GetRotationAngle](./getrotationangle/) | Rappresenta l'angolo di rotazione del testo. |
| [SetRotationAngle](./setrotationangle/) | Rappresenta l'angolo di rotazione del testo. |
| [IsAutomaticRotation](./isautomaticrotation/) | Indica se il testo del grafico è ruotato automaticamente. |
| [Characters](./characters/) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo. |
| [GetReadingOrder](./getreadingorder/) | Rappresenta l'ordine di lettura del testo. |
| [SetReadingOrder](./setreadingorder/) | Rappresenta l'ordine di lettura del testo. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo. |
| [GetLinkedSource](./getlinkedsource/) | Ottiene e imposta un riferimento al foglio di lavoro. |
| [SetLinkedSource](./setlinkedsource/) | Ottiene e imposta un riferimento al foglio di lavoro. |
