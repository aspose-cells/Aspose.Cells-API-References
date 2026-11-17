---
title: "PageSetup Class"
linktitle: "PageSetup"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "PageSetup class. Incapsula l'oggetto che rappresenta pagesetup in Go."
type: docs
weight: 200
url: /it/go-cpp/pagesetup/
---

## PageSetup class

Incapsula l'oggetto che rappresenta la descrizione dell'impostazione della pagina. L'oggetto PageSetup contiene tutte le opzioni di impostazione della pagina.

```go

type PageSetup struct  {
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
| [GetODSPageBackground](./getodspagebackground/) | Ottiene lo sfondo di ODS. |
| [Copy](./copy/) | Copia le impostazioni della configurazione della pagina. |
| [GetPrintArea](./getprintarea/) | Rappresenta l'intervallo da stampare. |
| [SetPrintArea](./setprintarea/) | Rappresenta l'intervallo da stampare. |
| [GetPrintTitleColumns](./getprinttitlecolumns/) | Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina. |
| [SetPrintTitleColumns](./setprinttitlecolumns/) | Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina. |
| [GetPrintTitleRows](./getprinttitlerows/) | Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina. |
| [SetPrintTitleRows](./setprinttitlerows/) | Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina. |
| [GetBlackAndWhite](./getblackandwhite/) | Rappresenta se gli elementi del documento saranno stampati in bianco e nero. |
| [SetBlackAndWhite](./setblackandwhite/) | Rappresenta se gli elementi del documento saranno stampati in bianco e nero. |
| [GetCenterHorizontally](./getcenterhorizontally/) | Rappresenta se il foglio è stampato centrato orizzontalmente. |
| [SetCenterHorizontally](./setcenterhorizontally/) | Rappresenta se il foglio è stampato centrato orizzontalmente. |
| [GetCenterVertically](./getcentervertically/) | Rappresenta se il foglio viene stampato centrato verticalmente. |
| [SetCenterVertically](./setcentervertically/) | Rappresenta se il foglio viene stampato centrato verticalmente. |
| [GetPrintDraft](./getprintdraft/) | Rappresenta se il foglio verrà stampato senza grafica. |
| [SetPrintDraft](./setprintdraft/) | Rappresenta se il foglio verrà stampato senza grafica. |
| [GetFooterMargin](./getfootermargin/) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di centimetri. |
| [SetFooterMargin](./setfootermargin/) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di centimetri. |
| [GetFooterMarginInch](./getfootermargininch/) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di pollici. |
| [SetFooterMarginInch](./setfootermargininch/) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di pollici. |
| [GetHeaderMargin](./getheadermargin/) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di centimetri. |
| [SetHeaderMargin](./setheadermargin/) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di centimetri. |
| [GetHeaderMarginInch](./getheadermargininch/) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di pollici. |
| [SetHeaderMarginInch](./setheadermargininch/) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di pollici. |
| [GetPrinterSettings](./getprintersettings/) | Ottiene e imposta le impostazioni della stampante predefinita. |
| [SetPrinterSettings](./setprintersettings/) | Ottiene e imposta le impostazioni della stampante predefinita. |
| [GetLeftMargin](./getleftmargin/) | Rappresenta la dimensione del margine sinistro, in unità di centimetri. |
| [SetLeftMargin](./setleftmargin/) | Rappresenta la dimensione del margine sinistro, in unità di centimetri. |
| [GetLeftMarginInch](./getleftmargininch/) | Rappresenta la dimensione del margine sinistro, in unità di pollici. |
| [SetLeftMarginInch](./setleftmargininch/) | Rappresenta la dimensione del margine sinistro, in unità di pollici. |
| [GetRightMargin](./getrightmargin/) | Rappresenta la dimensione del margine destro, in unità di centimetri. |
| [SetRightMargin](./setrightmargin/) | Rappresenta la dimensione del margine destro, in unità di centimetri. |
| [GetRightMarginInch](./getrightmargininch/) | Rappresenta la dimensione del margine destro, in unità di pollici. |
| [SetRightMarginInch](./setrightmargininch/) | Rappresenta la dimensione del margine destro, in unità di pollici. |
| [GetTopMargin](./gettopmargin/) | Rappresenta la dimensione del margine superiore, in unità di centimetri. |
| [SetTopMargin](./settopmargin/) | Rappresenta la dimensione del margine superiore, in unità di centimetri. |
| [GetTopMarginInch](./gettopmargininch/) | Rappresenta la dimensione del margine superiore, in unità di pollici. |
| [SetTopMarginInch](./settopmargininch/) | Rappresenta la dimensione del margine superiore, in unità di pollici. |
| [GetBottomMargin](./getbottommargin/) | Rappresenta la dimensione del margine inferiore, in unità di centimetri. |
| [SetBottomMargin](./setbottommargin/) | Rappresenta la dimensione del margine inferiore, in unità di centimetri. |
| [GetBottomMarginInch](./getbottommargininch/) | Rappresenta la dimensione del margine inferiore, in unità di pollici. |
| [SetBottomMarginInch](./setbottommargininch/) | Rappresenta la dimensione del margine inferiore, in unità di pollici. |
| [GetFirstPageNumber](./getfirstpagenumber/) | Rappresenta il numero della prima pagina che verrà usato quando questo foglio è stampato. |
| [SetFirstPageNumber](./setfirstpagenumber/) | Rappresenta il numero della prima pagina che verrà usato quando questo foglio è stampato. |
| [SetFitToPages](./setfittopages/) | Imposta il numero di pagine a cui il foglio di lavoro sarà scalato quando viene stampato. |
| [GetFitToPagesTall](./getfittopagestall/) | Rappresenta il numero di pagine in altezza a cui il foglio di lavoro sarà scalato quando viene stampato. Il valore predefinito è 1. |
| [SetFitToPagesTall](./setfittopagestall/) | Rappresenta il numero di pagine in altezza a cui il foglio di lavoro sarà scalato quando viene stampato. Il valore predefinito è 1. |
| [GetFitToPagesWide](./getfittopageswide/) | Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro sarà scalato quando viene stampato. Il valore predefinito è 1. |
| [SetFitToPagesWide](./setfittopageswide/) | Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro sarà scalato quando viene stampato. Il valore predefinito è 1. |
| [IsPercentScale](./ispercentscale/) | Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come il foglio di lavoro è scalato. |
| [SetIsPercentScale](./setispercentscale/) | Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come il foglio di lavoro è scalato. |
| [GetOrder](./getorder/) | Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine quando stampa un foglio di lavoro di grandi dimensioni. |
| [SetOrder](./setorder/) | Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine quando stampa un foglio di lavoro di grandi dimensioni. |
| [IsAutomaticPaperSize](./isautomaticpapersize/) | Indica se la dimensione della carta è automatica. |
| [GetPaperSize](./getpapersize/) | Rappresenta la dimensione della carta. |
| [SetPaperSize](./setpapersize/) | Rappresenta la dimensione della carta. |
| [GetPaperWidth](./getpaperwidth/) | Ottiene la larghezza della carta in unità di pollici, considerando l'orientamento della pagina. |
| [GetPaperHeight](./getpaperheight/) | Ottiene l'altezza della carta in unità di pollici, considerando l'orientamento della pagina. |
| [CustomPaperSize](./custompapersize/) | Imposta la dimensione personalizzata della carta, in unità di pollici. |
| [GetOrientation](./getorientation/) | Rappresenta l'orientamento di stampa della pagina. |
| [SetOrientation](./setorientation/) | Rappresenta l'orientamento di stampa della pagina. |
| [GetPrintComments](./getprintcomments/) | Rappresenta il modo in cui i commenti vengono stampati con il foglio. |
| [SetPrintComments](./setprintcomments/) | Rappresenta il modo in cui i commenti vengono stampati con il foglio. |
| [GetPrintErrors](./getprinterrors/) | Specifica il tipo di errore di stampa visualizzato. |
| [SetPrintErrors](./setprinterrors/) | Specifica il tipo di errore di stampa visualizzato. |
| [GetPrintHeadings](./getprintheadings/) | Rappresenta se le intestazioni di righe e colonne sono stampate con questa pagina. |
| [SetPrintHeadings](./setprintheadings/) | Rappresenta se le intestazioni di righe e colonne sono stampate con questa pagina. |
| [GetPrintGridlines](./getprintgridlines/) | Rappresenta se le linee della griglia delle celle sono stampate sulla pagina. |
| [SetPrintGridlines](./setprintgridlines/) | Rappresenta se le linee della griglia delle celle sono stampate sulla pagina. |
| [GetZoom](./getzoom/) | Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400. |
| [SetZoom](./setzoom/) | Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400. |
| [IsAutoFirstPageNumber](./isautofirstpagenumber/) | Indica se il numero della prima pagina è assegnato automaticamente. |
| [SetIsAutoFirstPageNumber](./setisautofirstpagenumber/) | Indica se il numero della prima pagina è assegnato automaticamente. |
| [GetPrintQuality](./getprintquality/) | Rappresenta la qualità di stampa. |
| [SetPrintQuality](./setprintquality/) | Rappresenta la qualità di stampa. |
| [GetPrintCopies](./getprintcopies/) | Ottiene e imposta il numero di copie da stampare. |
| [SetPrintCopies](./setprintcopies/) | Ottiene e imposta il numero di copie da stampare. |
| [ClearHeaderFooter](./clearheaderfooter/) | Cancella le impostazioni di intestazione e piè di pagina. |
| [GetHeader](./getheader/) | Ottiene uno script che formatta l'intestazione di un file Excel. |
| [GetCommands](./getcommands/) | Ottiene tutti i comandi dell'intestazione o del piè di pagina. |
| [GetFooter](./getfooter/) | Ottiene uno script che formatta il piè di pagina di un file Excel. |
| [SetHeader](./setheader/) | Imposta uno script che formatta l'intestazione di un file Excel. |
| [SetFooter](./setfooter/) | Imposta uno script che formatta il piè di pagina di un file Excel. |
| [SetEvenHeader](./setevenheader/) | Imposta uno script che formatta l'intestazione delle pagine pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è true. |
| [GetEvenHeader](./getevenheader/) | Ottiene uno script che formatta l'intestazione delle pagine pari di un file Excel. |
| [SetEvenFooter](./setevenfooter/) | Imposta uno script che formatta il piè di pagina delle pagine pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è true. |
| [GetEvenFooter](./getevenfooter/) | Ottiene uno script che formatta il piè di pagina delle pagine pari di un file Excel. |
| [SetFirstPageHeader](./setfirstpageheader/) | Imposta uno script che formatta l'intestazione della prima pagina di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffFirst è true. |
| [GetFirstPageHeader](./getfirstpageheader/) | Ottiene uno script che formatta l'intestazione della prima pagina di un file Excel. |
| [SetFirstPageFooter](./setfirstpagefooter/) | Imposta uno script che formatta il piè di pagina della prima pagina di un file Excel. |
| [GetFirstPageFooter](./getfirstpagefooter/) | Ottiene uno script che formatta il piè di pagina della prima pagina di un file Excel. |
| [IsHFDiffOddEven](./ishfdiffoddeven/) | True indica che l'intestazione/piè di pagina delle pagine dispari è diversa da quelle pari. |
| [SetIsHFDiffOddEven](./setishfdiffoddeven/) | True indica che l'intestazione/piè di pagina delle pagine dispari è diversa da quelle pari. |
| [IsHFDiffFirst](./ishfdifffirst/) | True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine. |
| [SetIsHFDiffFirst](./setishfdifffirst/) | True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine. |
| [IsHFScaleWithDoc](./ishfscalewithdoc/) | Indica se intestazione e piè di pagina sono scalati con la scala del documento. Si applica solo a Excel 2007. |
| [SetIsHFScaleWithDoc](./setishfscalewithdoc/) | Indica se intestazione e piè di pagina sono scalati con la scala del documento. Si applica solo a Excel 2007. |
| [IsHFAlignMargins](./ishfalignmargins/) | Indica se i margini di intestazione e piè di pagina sono allineati ai margini della pagina. Se questa proprietà è true, l'intestazione e il piè di pagina sinistro saranno allineati al margine sinistro, e quelli destro saranno allineati al margine destro. Questa opzione è abilitata per impostazione predefinita. |
| [SetIsHFAlignMargins](./setishfalignmargins/) | Indica se i margini di intestazione e piè di pagina sono allineati ai margini della pagina. Se questa proprietà è true, l'intestazione e il piè di pagina sinistro saranno allineati al margine sinistro, e quelli destro saranno allineati al margine destro. Questa opzione è abilitata per impostazione predefinita. |
| [SetHeaderPicture](./setheaderpicture/) | Imposta un'immagine nell'intestazione di un foglio di lavoro. |
| [SetFooterPicture](./setfooterpicture/) | Imposta un'immagine nel piè di pagina di un foglio di lavoro. |
| [SetPicture](./setpicture/) | Imposta un'immagine nell'intestazione/piè di pagina di un foglio di lavoro. |
| [GetPicture_Bool_Int](./getpicture_bool_int/) | Ottiene l'oggetto Picture dell'intestazione / piè di pagina. |
| [GetPicture_Bool_Bool_Bool_Int](./getpicture_bool_bool_bool_int/) | Ottiene l'oggetto Picture dell'intestazione / piè di pagina. |
