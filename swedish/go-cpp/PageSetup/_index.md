---
title: "PageSetup klass"
linktitle: "PageSetup"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PageSetup klass. Inkapslar objektet som representerar pagesetup i Go."
type: docs
weight: 200
url: /sv/go-cpp/pagesetup/
---

## PageSetup class

Inkapslar objektet som representerar sidinställningsbeskrivningen. PageSetup-objektet innehåller alla sidinställningsalternativ.

```go

type PageSetup struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetODSPageBackground](./getodspagebackground/) | Hämtar bakgrunden för ODS. |
| [Copy](./copy/) | Kopierar inställningen för sidinställningen. |
| [GetPrintArea](./getprintarea/) | Representerar intervallet som ska skrivas ut. |
| [SetPrintArea](./setprintarea/) | Representerar intervallet som ska skrivas ut. |
| [GetPrintTitleColumns](./getprinttitlecolumns/) | Representerar kolumnerna som innehåller cellerna som ska upprepas på vänster sida av varje sida. |
| [SetPrintTitleColumns](./setprinttitlecolumns/) | Representerar kolumnerna som innehåller cellerna som ska upprepas på vänster sida av varje sida. |
| [GetPrintTitleRows](./getprinttitlerows/) | Representerar raderna som innehåller cellerna som ska upprepas högst upp på varje sida. |
| [SetPrintTitleRows](./setprinttitlerows/) | Representerar raderna som innehåller cellerna som ska upprepas högst upp på varje sida. |
| [GetBlackAndWhite](./getblackandwhite/) | Representerar om element i dokumentet kommer att skrivas ut i svartvitt. |
| [SetBlackAndWhite](./setblackandwhite/) | Representerar om element i dokumentet kommer att skrivas ut i svartvitt. |
| [GetCenterHorizontally](./getcenterhorizontally/) | Representerar om bladet skrivs ut centrerat horisontellt. |
| [SetCenterHorizontally](./setcenterhorizontally/) | Representerar om bladet skrivs ut centrerat horisontellt. |
| [GetCenterVertically](./getcentervertically/) | Representerar om bladet skrivs ut centrerat vertikalt. |
| [SetCenterVertically](./setcentervertically/) | Representerar om bladet skrivs ut centrerat vertikalt. |
| [GetPrintDraft](./getprintdraft/) | Representerar om bladet ska skrivas ut utan grafik. |
| [SetPrintDraft](./setprintdraft/) | Representerar om bladet ska skrivas ut utan grafik. |
| [GetFooterMargin](./getfootermargin/) | Representerar avståndet från sidans botten till sidfoten, i centimeter. |
| [SetFooterMargin](./setfootermargin/) | Representerar avståndet från sidans botten till sidfoten, i centimeter. |
| [GetFooterMarginInch](./getfootermargininch/) | Representerar avståndet från sidans botten till sidfoten, i tum. |
| [SetFooterMarginInch](./setfootermargininch/) | Representerar avståndet från sidans botten till sidfoten, i tum. |
| [GetHeaderMargin](./getheadermargin/) | Representerar avståndet från sidans topp till sidhuvudet, i centimeter. |
| [SetHeaderMargin](./setheadermargin/) | Representerar avståndet från sidans topp till sidhuvudet, i centimeter. |
| [GetHeaderMarginInch](./getheadermargininch/) | Representerar avståndet från sidans topp till sidhuvudet, i tum. |
| [SetHeaderMarginInch](./setheadermargininch/) | Representerar avståndet från sidans topp till sidhuvudet, i tum. |
| [GetPrinterSettings](./getprintersettings/) | Hämtar och anger inställningarna för standardskrivaren. |
| [SetPrinterSettings](./setprintersettings/) | Hämtar och anger inställningarna för standardskrivaren. |
| [GetLeftMargin](./getleftmargin/) | Representerar storleken på vänstermarginalen, i centimeter. |
| [SetLeftMargin](./setleftmargin/) | Representerar storleken på vänstermarginalen, i centimeter. |
| [GetLeftMarginInch](./getleftmargininch/) | Representerar storleken på vänstermarginalen, i tum. |
| [SetLeftMarginInch](./setleftmargininch/) | Representerar storleken på vänstermarginalen, i tum. |
| [GetRightMargin](./getrightmargin/) | Representerar storleken på högermarginalen, i centimeter. |
| [SetRightMargin](./setrightmargin/) | Representerar storleken på högermarginalen, i centimeter. |
| [GetRightMarginInch](./getrightmargininch/) | Representerar storleken på högermarginalen, i tum. |
| [SetRightMarginInch](./setrightmargininch/) | Representerar storleken på högermarginalen, i tum. |
| [GetTopMargin](./gettopmargin/) | Representerar storleken på övre marginalen, i centimeter. |
| [SetTopMargin](./settopmargin/) | Representerar storleken på övre marginalen, i centimeter. |
| [GetTopMarginInch](./gettopmargininch/) | Representerar storleken på övre marginalen, i tum. |
| [SetTopMarginInch](./settopmargininch/) | Representerar storleken på övre marginalen, i tum. |
| [GetBottomMargin](./getbottommargin/) | Representerar storleken på nedre marginalen, i centimeter. |
| [SetBottomMargin](./setbottommargin/) | Representerar storleken på nedre marginalen, i centimeter. |
| [GetBottomMarginInch](./getbottommargininch/) | Representerar storleken på nedre marginalen, i tum. |
| [SetBottomMarginInch](./setbottommargininch/) | Representerar storleken på nedre marginalen, i tum. |
| [GetFirstPageNumber](./getfirstpagenumber/) | Representerar det första sidnumret som kommer att användas när detta blad skrivs ut. |
| [SetFirstPageNumber](./setfirstpagenumber/) | Representerar det första sidnumret som kommer att användas när detta blad skrivs ut. |
| [SetFitToPages](./setfittopages/) | Ställer in antalet sidor som arbetsbladet kommer att skalas till när det skrivs ut. |
| [GetFitToPagesTall](./getfittopagestall/) | Representerar antalet sidor i höjd som arbetsbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1. |
| [SetFitToPagesTall](./setfittopagestall/) | Representerar antalet sidor i höjd som arbetsbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1. |
| [GetFitToPagesWide](./getfittopageswide/) | Representerar antalet sidor i bredd som arbetsbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1. |
| [SetFitToPagesWide](./setfittopageswide/) | Representerar antalet sidor i bredd som arbetsbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1. |
| [IsPercentScale](./ispercentscale/) | Om den här egenskapen är falsk styr egenskaperna FitToPagesWide och FitToPagesTall hur arbetsbladet skalas. |
| [SetIsPercentScale](./setispercentscale/) | Om den här egenskapen är falsk styr egenskaperna FitToPagesWide och FitToPagesTall hur arbetsbladet skalas. |
| [GetOrder](./getorder/) | Representerar den ordning som Microsoft Excel använder för att numrera sidor när ett stort arbetsblad skrivs ut. |
| [SetOrder](./setorder/) | Representerar den ordning som Microsoft Excel använder för att numrera sidor när ett stort arbetsblad skrivs ut. |
| [IsAutomaticPaperSize](./isautomaticpapersize/) | Anger om papperstorleken är automatisk. |
| [GetPaperSize](./getpapersize/) | Representerar papperets storlek. |
| [SetPaperSize](./setpapersize/) | Representerar papperets storlek. |
| [GetPaperWidth](./getpaperwidth/) | Hämtar papperets bredd i tum, med hänsyn till sidorientering. |
| [GetPaperHeight](./getpaperheight/) | Hämtar papperets höjd i tum, med hänsyn till sidorientering. |
| [CustomPaperSize](./custompapersize/) | Ställer in den anpassade papperstorleken i tum. |
| [GetOrientation](./getorientation/) | Representerar sidans utskriftsorientering. |
| [SetOrientation](./setorientation/) | Representerar sidans utskriftsorientering. |
| [GetPrintComments](./getprintcomments/) | Representerar hur kommentarer skrivs ut med bladet. |
| [SetPrintComments](./setprintcomments/) | Representerar hur kommentarer skrivs ut med bladet. |
| [GetPrintErrors](./getprinterrors/) | Anger typen av utskriftsfel som visas. |
| [SetPrintErrors](./setprinterrors/) | Anger typen av utskriftsfel som visas. |
| [GetPrintHeadings](./getprintheadings/) | Representerar om rad- och kolumnrubriker skrivs ut på den här sidan. |
| [SetPrintHeadings](./setprintheadings/) | Representerar om rad- och kolumnrubriker skrivs ut på den här sidan. |
| [GetPrintGridlines](./getprintgridlines/) | Representerar om cellrutnät skrivs ut på sidan. |
| [SetPrintGridlines](./setprintgridlines/) | Representerar om cellrutnät skrivs ut på sidan. |
| [GetZoom](./getzoom/) | Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400. |
| [SetZoom](./setzoom/) | Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400. |
| [IsAutoFirstPageNumber](./isautofirstpagenumber/) | Anger om det första sidnumret tilldelas automatiskt. |
| [SetIsAutoFirstPageNumber](./setisautofirstpagenumber/) | Anger om det första sidnumret tilldelas automatiskt. |
| [GetPrintQuality](./getprintquality/) | Representerar utskriftskvaliteten. |
| [SetPrintQuality](./setprintquality/) | Representerar utskriftskvaliteten. |
| [GetPrintCopies](./getprintcopies/) | Hämtar och ställer in antalet kopior som ska skrivas ut. |
| [SetPrintCopies](./setprintcopies/) | Hämtar och ställer in antalet kopior som ska skrivas ut. |
| [ClearHeaderFooter](./clearheaderfooter/) | Rensar inställningarna för sidhuvud och sidfot. |
| [GetHeader](./getheader/) | Hämtar ett skript som formaterar sidhuvudet i en Excel-fil. |
| [GetCommands](./getcommands/) | Hämtar alla kommandon för sidhuvud eller sidfot. |
| [GetFooter](./getfooter/) | Hämtar ett skript som formaterar sidfoten i en Excel-fil. |
| [SetHeader](./setheader/) | Ställer in ett skript som formaterar sidhuvudet i en Excel-fil. |
| [SetFooter](./setfooter/) | Ställer in ett skript som formaterar sidfoten i en Excel-fil. |
| [SetEvenHeader](./setevenheader/) | Ställer in ett skript som formaterar jämna sidhuvudet i en Excel‑fil. Gäller endast i Excel 2007 när IsHFDiffOddEven är sant. |
| [GetEvenHeader](./getevenheader/) | Hämtar ett skript som formaterar det jämna sidhuvudet i en Excel‑fil. |
| [SetEvenFooter](./setevenfooter/) | Ställer in ett skript som formaterar jämna sidfoten i en Excel‑fil. Gäller endast i Excel 2007 när IsHFDiffOddEven är sant. |
| [GetEvenFooter](./getevenfooter/) | Hämtar ett skript som formaterar den jämna sidfoten i en Excel‑fil. |
| [SetFirstPageHeader](./setfirstpageheader/) | Ställer in ett skript som formaterar första sidhuvudet i en Excel‑fil. Gäller endast i Excel 2007 när IsHFDiffFirst är sant. |
| [GetFirstPageHeader](./getfirstpageheader/) | Hämtar ett skript som formaterar det första sidhuvudet i en Excel‑fil. |
| [SetFirstPageFooter](./setfirstpagefooter/) | Ställer in ett skript som formaterar den första sidfoten i en Excel‑fil. |
| [GetFirstPageFooter](./getfirstpagefooter/) | Hämtar ett skript som formaterar den första sidfoten i en Excel‑fil. |
| [IsHFDiffOddEven](./ishfdiffoddeven/) | Sant betyder att sidhuvudet/sidfoten för udda sidor är olika jämfört med udda sidor. |
| [SetIsHFDiffOddEven](./setishfdiffoddeven/) | Sant betyder att sidhuvudet/sidfoten för udda sidor är olika jämfört med udda sidor. |
| [IsHFDiffFirst](./ishfdifffirst/) | Sant betyder att sidhuvudet/sidfoten för den första sidan är olika jämfört med andra sidor. |
| [SetIsHFDiffFirst](./setishfdifffirst/) | Sant betyder att sidhuvudet/sidfoten för den första sidan är olika jämfört med andra sidor. |
| [IsHFScaleWithDoc](./ishfscalewithdoc/) | Anger om sidhuvudet och sidfoten skalas med dokumentets skalning. Gäller endast för Excel 2007. |
| [SetIsHFScaleWithDoc](./setishfscalewithdoc/) | Anger om sidhuvudet och sidfoten skalas med dokumentets skalning. Gäller endast för Excel 2007. |
| [IsHFAlignMargins](./ishfalignmargins/) | Anger om marginalerna för sidhuvud och sidfot är anpassade till sidmarginalerna. Om denna egenskap är sann kommer vänstra sidhuvudet och sidfoten att justeras med den vänstra marginalen, och högra sidhuvudet och sidfoten med den högra marginalen. Detta alternativ är aktiverat som standard. |
| [SetIsHFAlignMargins](./setishfalignmargins/) | Anger om marginalerna för sidhuvud och sidfot är anpassade till sidmarginalerna. Om denna egenskap är sann kommer vänstra sidhuvudet och sidfoten att justeras med den vänstra marginalen, och högra sidhuvudet och sidfoten med den högra marginalen. Detta alternativ är aktiverat som standard. |
| [SetHeaderPicture](./setheaderpicture/) | Ställer in en bild i sidhuvudet på ett arbetsblad. |
| [SetFooterPicture](./setfooterpicture/) | Ställer in en bild i sidfoten på ett arbetsblad. |
| [SetPicture](./setpicture/) | Ställer in en bild i sidhuvudet/sidfoten på ett arbetsblad. |
| [GetPicture_Bool_Int](./getpicture_bool_int/) | Hämtar Picture‑objektet för sidhuvudet / sidfoten. |
| [GetPicture_Bool_Bool_Bool_Int](./getpicture_bool_bool_bool_int/) | Hämtar Picture‑objektet för sidhuvudet / sidfoten. |
