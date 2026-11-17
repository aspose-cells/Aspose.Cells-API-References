---
title: "Chart Classe"
linktitle: "Chart"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Chart class. Incapsula l'oggetto che rappresenta chart in Go."
type: docs
weight: 200
url: /it/go-cpp/chart/
---

## Chart class

Incapsula l'oggetto che rappresenta un singolo grafico Excel.

```go

type Chart struct  {
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
| [GetStyle](./getstyle/) | Ottiene e imposta lo stile predefinito. |
| [SetStyle](./setstyle/) | Ottiene e imposta lo stile predefinito. |
| [GetChartObject](./getchartobject/) | Rappresenta il chartShape; |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è PivotChart. |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è PivotChart. |
| [GetPivotOptions](./getpivotoptions/) | Specifica i controlli pivot che appaiono sul grafico |
| [GetPivotSource](./getpivotsource/) | La sorgente è i dati della tabella pivot. Se PivotSource non è vuoto, il grafico è PivotChart. |
| [SetPivotSource](./setpivotsource/) | La sorgente è i dati della tabella pivot. Se PivotSource non è vuoto, il grafico è PivotChart. |
| [IsCellReferedByChart](./iscellreferedbychart/) | Restituisce se la cella a cui si riferisce il grafico. |
| [IsChartDataChanged](./ischartdatachanged/) | Rileva se la fonte dati di un grafico è cambiata. |
| [GetPlotBy](./getplotby/) | Ottiene e imposta se tracciare per riga o per colonna. |
| [RefreshPivotData](./refreshpivotdata/) | Aggiorna i dati del grafico dalla tabella pivot. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Ottiene e imposta come tracciare le celle vuote. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Ottiene e imposta come tracciare le celle vuote. |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | Indica se tracciare solo le celle visibili. |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | Indica se tracciare solo le celle visibili. |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | Indica se visualizzare #N/A come valore vuoto. |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | Indica se visualizzare #N/A come valore vuoto. |
| [GetName](./getname/) | Ottiene e imposta il nome del grafico. |
| [SetName](./setname/) | Ottiene e imposta il nome del grafico. |
| [GetSizeWithWindow](./getsizewithwindow/) | Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico. |
| [SetSizeWithWindow](./setsizewithwindow/) | Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico. |
| [GetWorksheet](./getworksheet/) | Ottiene il foglio di lavoro che contiene questo grafico. |
| [GetShapes](./getshapes/) | Restituisce tutte le forme di disegno in questo grafico. |
| [GetPrintSize](./getprintsize/) | Ottiene e imposta la dimensione del grafico stampato. |
| [SetPrintSize](./setprintsize/) | Ottiene e imposta la dimensione del grafico stampato. |
| [ChangeTemplate](./changetemplate/) | Modifica il tipo di grafico con un modello predefinito. |
| [GetType](./gettype/) | Ottiene o imposta il tipo di un grafico. |
| [SetType](./settype/) | Ottiene o imposta il tipo di un grafico. |
| [Move](./move/) | Sposta il grafico in una posizione specificata. |
| [GetNSeries](./getnseries/) | Ottiene una collezione SeriesCollection che rappresenta le serie di dati nel grafico. |
| [GetFilteredNSeries](./getfilterednseries/) | Ottiene una collezione SeriesCollection che rappresenta le serie di dati filtrate nel grafico. |
| [GetTitle](./gettitle/) | Ottiene il titolo del grafico. |
| [GetSubTitle](./getsubtitle/) | Ottiene il sottotitolo del grafico. Si applica solo ai file ODS. |
| [GetPlotArea](./getplotarea/) | Ottiene l'area di tracciamento del grafico che include le etichette di graduazione degli assi. |
| [GetChartArea](./getchartarea/) | Ottiene l'area del grafico nel foglio di lavoro. |
| [GetCategoryAxis](./getcategoryaxis/) | Ottiene l'asse X del grafico. |
| [GetValueAxis](./getvalueaxis/) | Ottiene l'asse Y del grafico. |
| [GetSecondValueAxis](./getsecondvalueaxis/) | Ottiene il secondo asse Y del grafico. |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | Ottiene il secondo asse X del grafico. |
| [GetSeriesAxis](./getseriesaxis/) | Ottiene l'asse delle serie del grafico. |
| [GetLegend](./getlegend/) | Ottiene la legenda del grafico. |
| [GetChartDataTable](./getchartdatatable/) | Rappresenta la tabella dei dati del grafico. |
| [GetShowLegend](./getshowlegend/) | Ottiene o imposta un valore che indica se la legenda del grafico deve essere visualizzata. Il valore predefinito è true. |
| [SetShowLegend](./setshowlegend/) | Ottiene o imposta un valore che indica se la legenda del grafico deve essere visualizzata. Il valore predefinito è true. |
| [IsRectangularCornered](./isrectangularcornered/) | Ottiene o imposta un valore che indica se l'area del grafico ha angoli rettangolari. Il valore predefinito è true. |
| [SetIsRectangularCornered](./setisrectangularcornered/) | Ottiene o imposta un valore che indica se l'area del grafico ha angoli rettangolari. Il valore predefinito è true. |
| [GetShowDataTable](./getshowdatatable/) | Ottiene o imposta un valore che indica se il grafico visualizza una tabella dei dati. |
| [SetShowDataTable](./setshowdatatable/) | Ottiene o imposta un valore che indica se il grafico visualizza una tabella dei dati. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Ottiene o imposta l'angolo della prima fetta di un grafico a torta o a ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3D e a ciambella, da 0 a 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Ottiene o imposta l'angolo della prima fetta di un grafico a torta o a ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3D e a ciambella, da 0 a 360. |
| [GetGapWidth](./getgapwidth/) | Restituisce o imposta lo spazio tra i gruppi di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [SetGapWidth](./setgapwidth/) | Restituisce o imposta lo spazio tra i gruppi di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [GetGapDepth](./getgapdepth/) | Ottiene o imposta la distanza tra le serie di dati in un grafico 3D, come percentuale della larghezza del marcatore. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [SetGapDepth](./setgapdepth/) | Ottiene o imposta la distanza tra le serie di dati in un grafico 3D, come percentuale della larghezza del marcatore. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [Calculate](./calculate/) | Calcola le posizioni personalizzate dell'area di tracciamento e degli assi se le loro posizioni sono assegnate automaticamente. |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | Calcola la posizione personalizzata dell'area del grafico, degli assi se la loro posizione è assegnata automaticamente, con le Opzioni di Calcolo del Grafico. |
| [GetFloor](./getfloor/) | Restituisce un oggetto Floor che rappresenta le pareti di un grafico 3-D. |
| [GetWalls](./getwalls/) | Restituisce un oggetto Walls che rappresenta le pareti di un grafico 3-D. |
| [GetBackWall](./getbackwall/) | Restituisce un oggetto Walls che rappresenta la parete posteriore di un grafico 3-D. |
| [GetSideWall](./getsidewall/) | Restituisce un oggetto Walls che rappresenta la parete laterale di un grafico 3-D. |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D. |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D. |
| [GetRotationAngle](./getrotationangle/) | Rappresenta la rotazione della visualizzazione del grafico 3-D (la rotazione dell'area del grafico attorno all'asse z, in gradi). |
| [SetRotationAngle](./setrotationangle/) | Rappresenta la rotazione della visualizzazione del grafico 3-D (la rotazione dell'area del grafico attorno all'asse z, in gradi). |
| [GetElevation](./getelevation/) | Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi. |
| [SetElevation](./setelevation/) | Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi. |
| [GetRightAngleAxes](./getrightangleaxes/) | Vero se gli assi del grafico sono perpendicolari. Si applica solo ai grafici 3-D (eccetto Column3D e grafici a torta 3-D). |
| [SetRightAngleAxes](./setrightangleaxes/) | Vero se gli assi del grafico sono perpendicolari. Si applica solo ai grafici 3-D (eccetto Column3D e grafici a torta 3-D). |
| [GetAutoScaling](./getautoscaling/) | Vero se Microsoft Excel scala un grafico 3-D in modo che sia più vicino in dimensione al grafico 2-D equivalente. La proprietà RightAngleAxes deve essere Vero. |
| [SetAutoScaling](./setautoscaling/) | Vero se Microsoft Excel scala un grafico 3-D in modo che sia più vicino in dimensione al grafico 2-D equivalente. La proprietà RightAngleAxes deve essere Vero. |
| [GetHeightPercent](./getheightpercent/) | Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5% e il 500%). |
| [SetHeightPercent](./setheightpercent/) | Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5% e il 500%). |
| [GetPerspective](./getperspective/) | Restituisce o imposta la prospettiva per la visualizzazione del grafico tridimensionale. Deve essere compresa tra 0 e 100. Questa proprietà è ignorata se la proprietà RightAngleAxes è Vero. |
| [SetPerspective](./setperspective/) | Restituisce o imposta la prospettiva per la visualizzazione del grafico tridimensionale. Deve essere compresa tra 0 e 100. Questa proprietà è ignorata se la proprietà RightAngleAxes è Vero. |
| [GetIs3D](./getis3d/) | Indica se il grafico è un grafico 3D. |
| [GetDepthPercent](./getdepthpercent/) | Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20% e il 2000%). |
| [SetDepthPercent](./setdepthpercent/) | Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20% e il 2000%). |
| [ToImage_String](./toimage_string/) | Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine. |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | Crea l'immagine del grafico e la salva in un file del tipo di immagine specificato. |
| [ToImage_Int64](./toimage_int64/) | Crea l'immagine del grafico e la salva in uno stream in formato Jpeg. |
| [ToImage_ImageType](./toimage_imagetype/) | Crea l'immagine del grafico e la salva in uno stream nel formato specificato. |
| [ToPdf_String](./topdf_string/) | Salva il grafico in un file PDF. |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Salva il grafico in un file PDF. |
| [ToPdf](./topdf/) | Crea il PDF del grafico e lo salva in uno stream. |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Crea il PDF del grafico e lo salva in uno stream. |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine. |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Crea l'immagine del grafico e la salva in uno stream nel formato specificato. |
| [GetActualSize](./getactualsize/) | Restituisce la dimensione reale del grafico in unità di pixel. |
| [GetPlacement](./getplacement/) | Rappresenta il modo in cui il grafico è collegato alle celle sottostanti. |
| [SetPlacement](./setplacement/) | Rappresenta il modo in cui il grafico è collegato alle celle sottostanti. |
| [GetPageSetup](./getpagesetup/) | Rappresenta la descrizione dell'impostazione di pagina in questo grafico. |
| [HasAxis](./hasaxis/) | Restituisce quali assi esistono nel grafico. |
| [SwitchRowColumn](./switchrowcolumn/) | Scambia riga/colonna. |
| [GetChartDataRange](./getchartdatarange/) | Ottiene l'intervallo della fonte dati del grafico. |
| [SetChartDataRange](./setchartdatarange/) | Specifica l'intervallo dei dati per un grafico. |
| [GetLine](./getline/) | Ottiene la linea. |
