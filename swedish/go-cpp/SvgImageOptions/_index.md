---
title: "SvgImageOptions-klass"
linktitle: "SvgImageOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SvgImageOptions-klass. Inkapslar objektet som representerar svgimageoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/svgimageoptions/
---

## SvgImageOptions class

Alternativ för att generera SVG‑bild.

```go

type SvgImageOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewSvgImageOptions](./newsvgimageoptions/) | Konstruktor. |
| [NewSvgImageOptions_ImageOrPrintOptions](./newsvgimageoptions_imageorprintoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetImageType](./getimagetype/) | Hämtar eller sätter formatet för de genererade bilderna. Standardvärde: PNG. |
| [SetImageType](./setimagetype/) | Hämtar eller sätter formatet för de genererade bilderna. Standardvärde: PNG. |
| [GetFitToViewPort](./getfittoviewport/) | Om den här egenskapen är sann kommer den genererade SVG:n att anpassas till visningsporten. |
| [SetFitToViewPort](./setfittoviewport/) | Om den här egenskapen är sann kommer den genererade SVG:n att anpassas till visningsporten. |
| [GetCssPrefix](./getcssprefix/) | Hämtar och anger prefixet för css‑namnet i svg,standardvärdet är en tom sträng. |
| [SetCssPrefix](./setcssprefix/) | Hämtar och anger prefixet för css‑namnet i svg,standardvärdet är en tom sträng. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Hämtar eller anger teckensnittstypen som är inbäddad i Svg. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Hämtar eller anger teckensnittstypen som är inbäddad i Svg. |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | Om PrintWithStatusDialog = true , visas en dialog som visar aktuell utskriftsstatus. annars visas ingen sådan dialog. |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | Om PrintWithStatusDialog = true , visas en dialog som visar aktuell utskriftsstatus. annars visas ingen sådan dialog. |
| [GetHorizontalResolution](./gethorizontalresolution/) | Hämtar eller anger den horisontella upplösningen för genererade bilder, i punkter per tum. |
| [SetHorizontalResolution](./sethorizontalresolution/) | Hämtar eller anger den horisontella upplösningen för genererade bilder, i punkter per tum. |
| [GetVerticalResolution](./getverticalresolution/) | Hämtar eller anger den vertikala upplösningen för genererade bilder, i punkter per tum. |
| [SetVerticalResolution](./setverticalresolution/) | Hämtar eller anger den vertikala upplösningen för genererade bilder, i punkter per tum. |
| [GetTiffCompression](./gettiffcompression/) | Hämtar eller anger kompressionstypen som endast ska tillämpas när sidor sparas i <c>Tiff</c>-formatet. |
| [SetTiffCompression](./settiffcompression/) | Hämtar eller anger kompressionstypen som endast ska tillämpas när sidor sparas i <c>Tiff</c>-formatet. |
| [GetTiffColorDepth](./gettiffcolordepth/) | Hämtar eller anger bitdjupet som endast ska tillämpas när sidor sparas i <c>Tiff</c>-formatet. |
| [SetTiffColorDepth](./settiffcolordepth/) | Hämtar eller anger bitdjupet som endast ska tillämpas när sidor sparas i <c>Tiff</c>-formatet. |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | Hämtar eller anger metoden som används vid konvertering av bilder till 1 bpp-format när ImageType är Tiff och TiffCompression är lika med Ccitt3 eller Ccitt4. |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | Hämtar eller anger metoden som används vid konvertering av bilder till 1 bpp-format när ImageType är Tiff och TiffCompression är lika med Ccitt3 eller Ccitt4. |
| [GetPrintingPage](./getprintingpage/) | Anger vilka sidor som inte kommer att skrivas ut. |
| [SetPrintingPage](./setprintingpage/) | Anger vilka sidor som inte kommer att skrivas ut. |
| [GetQuality](./getquality/) | Hämtar eller anger ett värde som bestämmer kvaliteten på de genererade bilderna, som endast ska tillämpas när sidor sparas i <c>Jpeg</c>-formatet. Standardvärdet är 100 |
| [SetQuality](./setquality/) | Hämtar eller anger ett värde som bestämmer kvaliteten på de genererade bilderna, som endast ska tillämpas när sidor sparas i <c>Jpeg</c>-formatet. Standardvärdet är 100 |
| [GetOnePagePerSheet](./getonepagepersheet/) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Om AllColumnsInOnePagePerSheet är true, kommer allt kolumninnehåll på ett blad att skrivas ut på endast en sida i resultatet. Bredden på papperstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup gäller fortfarande. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Om AllColumnsInOnePagePerSheet är true, kommer allt kolumninnehåll på ett blad att skrivas ut på endast en sida i resultatet. Bredden på papperstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup gäller fortfarande. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [GetOnlyArea](./getonlyarea/) | Om denna egenskap är true, kommer ett område att skrivas ut och ingen skalning kommer att tillämpas. |
| [SetOnlyArea](./setonlyarea/) | Om denna egenskap är true, kommer ett område att skrivas ut och ingen skalning kommer att tillämpas. |
| [GetTransparent](./gettransparent/) | Anger om bakgrunden på den genererade bilden ska vara transparent. |
| [SetTransparent](./settransparent/) | Anger om bakgrunden på den genererade bilden ska vara transparent. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Anger om teckensnittet för ett tecken endast ska ersättas när cellens teckensnitt inte är kompatibelt med det. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Anger om teckensnittet för ett tecken endast ska ersättas när cellens teckensnitt inte är kompatibelt med det. |
| [SetPageIndex](./setpageindex/) | Hämtar eller anger det 0-baserade indexet för den första sidan som ska sparas. |
| [GetPageIndex](./getpageindex/) | Hämtar eller anger det 0-baserade indexet för den första sidan som ska sparas. |
| [SetPageCount](./setpagecount/) | Hämtar eller anger antalet sidor som ska sparas. |
| [GetPageCount](./getpagecount/) | Hämtar eller anger antalet sidor som ska sparas. |
| [SetDesiredSize](./setdesiredsize/) | Anger önskad bredd och höjd på bilden. |
| [IsOptimized](./isoptimized/) | Anger om utdataelementen ska optimeras. |
| [SetIsOptimized](./setisoptimized/) | Anger om utdataelementen ska optimeras. |
| [GetDefaultFont](./getdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken. |
| [SetDefaultFont](./setdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Sätt detta till true för att först försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf eller bild. Sätt detta till true för att först försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [GetGridlineType](./getgridlinetype/) | Hämtar eller anger rutnätslinjetyp. |
| [SetGridlineType](./setgridlinetype/) | Hämtar eller anger rutnätslinjetyp. |
| [GetGridlineColor](./getgridlinecolor/) | Hämtar eller anger rutnätsfärgen. |
| [SetGridlineColor](./setgridlinecolor/) | Hämtar eller anger rutnätsfärgen. |
| [GetTextCrossType](./gettextcrosstype/) | Hämtar eller anger visningstexttyp när textbredden är större än cellbredden. |
| [SetTextCrossType](./settextcrosstype/) | Hämtar eller anger visningstexttyp när textbredden är större än cellbredden. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Hämtar eller anger standardspråk för redigering. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Hämtar eller anger standardspråk för redigering. |
| [GetSheetSet](./getsheetset/) | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Inställning för rendering av Emf-metafiler i källfilen. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Inställning för rendering av Emf-metafiler i källfilen. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Hämtar eller anger anpassade inställningar under rendering. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Hämtar eller anger anpassade inställningar under rendering. |
