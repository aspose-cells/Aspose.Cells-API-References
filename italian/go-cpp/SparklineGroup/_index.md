---
title: "SparklineGroup Classe"
linktitle: "SparklineGroup"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe SparklineGroup. Incapsula l'oggetto che rappresenta sparklinegroup in Go."
type: docs
weight: 200
url: /it/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref=\"Sparkline\"/> è organizzato in un gruppo di sparkline. Un SparklineGroup contiene un numero variabile di elementi sparkline. Un gruppo di sparkline specifica il tipo, le impostazioni di visualizzazione e le impostazioni dell'asse per le sparkline.

```go

type SparklineGroup struct  {
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
| [ResetRanges](./resetranges/) | Reimposta l'intervallo dei dati e l'intervallo di posizione del gruppo sparkline. Questo metodo cancellerà gli elementi sparkline originali nel gruppo e creerà nuovi elementi sparkline per i nuovi intervalli. |
| [GetPresetStyle](./getpresetstyle/) | Ottiene e imposta il tipo di stile predefinito del gruppo sparkline. |
| [SetPresetStyle](./setpresetstyle/) | Ottiene e imposta il tipo di stile predefinito del gruppo sparkline. |
| [GetSparklines](./getsparklines/) | Ottiene la collezione di oggetti Sparkline. |
| [GetType](./gettype/) | Indica il tipo di sparkline del gruppo sparkline. |
| [SetType](./settype/) | Indica il tipo di sparkline del gruppo sparkline. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Indica come tracciare le celle vuote. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Indica come tracciare le celle vuote. |
| [GetDisplayHidden](./getdisplayhidden/) | Indica se mostrare i dati in righe e colonne nascoste. |
| [SetDisplayHidden](./setdisplayhidden/) | Indica se mostrare i dati in righe e colonne nascoste. |
| [GetShowHighPoint](./getshowhighpoint/) | Indica se evidenziare i punti più alti dei dati nel gruppo sparkline. |
| [SetShowHighPoint](./setshowhighpoint/) | Indica se evidenziare i punti più alti dei dati nel gruppo sparkline. |
| [GetHighPointColor](./gethighpointcolor/) | Ottiene e imposta il colore dei punti più alti dei dati nel gruppo sparkline. |
| [SetHighPointColor](./sethighpointcolor/) | Ottiene e imposta il colore dei punti più alti dei dati nel gruppo sparkline. |
| [GetShowLowPoint](./getshowlowpoint/) | Indica se evidenziare i punti più bassi dei dati nel gruppo sparkline. |
| [SetShowLowPoint](./setshowlowpoint/) | Indica se evidenziare i punti più bassi dei dati nel gruppo sparkline. |
| [GetLowPointColor](./getlowpointcolor/) | Ottiene e imposta il colore dei punti più bassi dei dati nel gruppo sparkline. |
| [SetLowPointColor](./setlowpointcolor/) | Ottiene e imposta il colore dei punti più bassi dei dati nel gruppo sparkline. |
| [GetShowNegativePoints](./getshownegativepoints/) | Indica se evidenziare i valori negativi nel gruppo sparkline con un colore o marcatore diverso. |
| [SetShowNegativePoints](./setshownegativepoints/) | Indica se evidenziare i valori negativi nel gruppo sparkline con un colore o marcatore diverso. |
| [GetNegativePointsColor](./getnegativepointscolor/) | Ottiene e imposta il colore dei valori negativi nel gruppo sparkline. |
| [SetNegativePointsColor](./setnegativepointscolor/) | Ottiene e imposta il colore dei valori negativi nel gruppo sparkline. |
| [GetShowFirstPoint](./getshowfirstpoint/) | Indica se evidenziare il primo punto dei dati nel gruppo sparkline. |
| [SetShowFirstPoint](./setshowfirstpoint/) | Indica se evidenziare il primo punto dei dati nel gruppo sparkline. |
| [GetFirstPointColor](./getfirstpointcolor/) | Ottiene e imposta il colore del primo punto dei dati nel gruppo sparkline. |
| [SetFirstPointColor](./setfirstpointcolor/) | Ottiene e imposta il colore del primo punto dei dati nel gruppo sparkline. |
| [GetShowLastPoint](./getshowlastpoint/) | Indica se evidenziare l'ultimo punto dei dati nel gruppo sparkline. |
| [SetShowLastPoint](./setshowlastpoint/) | Indica se evidenziare l'ultimo punto dei dati nel gruppo sparkline. |
| [GetLastPointColor](./getlastpointcolor/) | Ottiene e imposta il colore dell'ultimo punto dei dati nel gruppo sparkline. |
| [SetLastPointColor](./setlastpointcolor/) | Ottiene e imposta il colore dell'ultimo punto dei dati nel gruppo sparkline. |
| [GetShowMarkers](./getshowmarkers/) | Indica se evidenziare ogni punto in ogni sparkline a linee nel gruppo sparkline. |
| [SetShowMarkers](./setshowmarkers/) | Indica se evidenziare ogni punto in ogni sparkline a linee nel gruppo sparkline. |
| [GetMarkersColor](./getmarkerscolor/) | Ottiene e imposta il colore dei punti in ogni sparkline a linee nel gruppo sparkline. |
| [SetMarkersColor](./setmarkerscolor/) | Ottiene e imposta il colore dei punti in ogni sparkline a linee nel gruppo sparkline. |
| [GetSeriesColor](./getseriescolor/) | Ottiene e imposta il colore delle sparklines nel gruppo sparkline. |
| [SetSeriesColor](./setseriescolor/) | Ottiene e imposta il colore delle sparklines nel gruppo sparkline. |
| [GetPlotRightToLeft](./getplotrighttoleft/) | Indica se i dati del grafico sono da destra a sinistra. |
| [SetPlotRightToLeft](./setplotrighttoleft/) | Indica se i dati del grafico sono da destra a sinistra. |
| [GetLineWeight](./getlineweight/) | Ottiene e imposta lo spessore della linea in ogni sparkline a linee nel gruppo sparkline, nell'unità di punti. |
| [SetLineWeight](./setlineweight/) | Ottiene e imposta lo spessore della linea in ogni sparkline a linee nel gruppo sparkline, nell'unità di punti. |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | Ottiene e imposta il colore dell'asse orizzontale nel gruppo sparkline. |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | Ottiene e imposta il colore dell'asse orizzontale nel gruppo sparkline. |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | Indica se mostrare l'asse orizzontale dello sparkline.L'asse orizzontale appare se lo sparkline ha dati che attraversano l'asse zero. |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | Indica se mostrare l'asse orizzontale dello sparkline.L'asse orizzontale appare se lo sparkline ha dati che attraversano l'asse zero. |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | Rappresenta l'intervallo che contiene i valori di data per i dati dello sparkline. |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | Rappresenta l'intervallo che contiene i valori di data per i dati dello sparkline. |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | Rappresenta il tipo di valore massimo dell'asse verticale. |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | Rappresenta il tipo di valore massimo dell'asse verticale. |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | Ottiene e imposta il valore massimo personalizzato per l'asse verticale. |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | Ottiene e imposta il valore massimo personalizzato per l'asse verticale. |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | Imposta il valore massimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato. |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | Imposta il valore minimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato. |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | Rappresenta il tipo di valore minimo dell'asse verticale. |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | Rappresenta il tipo di valore minimo dell'asse verticale. |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | Ottiene e imposta il valore minimo personalizzato per l'asse verticale. |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | Ottiene e imposta il valore minimo personalizzato per l'asse verticale. |
