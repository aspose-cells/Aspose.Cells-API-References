---
title: "SvgImageOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Alternativ för att generera Svg-bild."
type: docs
url: /sv/java/com.aspose.cells/svgimageoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
```
public class SvgImageOptions extends ImageOrPrintOptions
```

Alternativ för att generera Svg-bild.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SvgImageOptions()](#SvgImageOptions--) | Konstruktor. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [getChartImageType()](#getChartImageType--) | Anger diagrammets bildtyp vid konvertering. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [getClass()](#getClass--) |  |
| [getCssPrefix()](#getCssPrefix--) | Hämtar prefixet för css-namnet i svg, standardvärdet är en tom sträng. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Hämtar anpassade inställningar under rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Hämtar standardspråk för redigering. |
| [getDefaultFont()](#getDefaultFont--) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Hämtar typen av teckensnitt som är inbäddad i Svg. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Anger filnamnet för den inbäddade bilden i svg. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Inställning för rendering av Emf-metafiler i källfilen. |
| [getFitToViewPort()](#getFitToViewPort--) | Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten. |
| [getGridlineColor()](#getGridlineColor--) | Hämtar rutnätslinjens färg. |
| [getGridlineType()](#getGridlineType--) | Hämtar typ av rutnätslinje. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Hämtar den horisontella upplösningen för genererade bilder, i punkter per tum. |
| [getImageType()](#getImageType--) | Hämtar formatet för de genererade bilderna. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [getOnlyArea()](#getOnlyArea--) | Om denna egenskap är sann, kommer ett område att skrivas ut, och ingen skala kommer att tillämpas. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [getPageCount()](#getPageCount--) | Hämtar antalet sidor som ska sparas. |
| [getPageIndex()](#getPageIndex--) | Hämtar det 0-baserade indexet för den första sidan som ska sparas. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Styr/indikera framsteg för sid sparningsprocessen. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | Om PrintWithStatusDialog = true, kommer en dialog att visas som visar aktuell utskriftsstatus. |
| [getPrintingPage()](#getPrintingPage--) | Anger vilka sidor som inte kommer att skrivas ut. |
| [getQuality()](#getQuality--) | Hämtar ett värde som bestämmer kvaliteten på de genererade bilderna, som endast tillämpas när sidor sparas i `Jpeg`-formatet. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatstypen för utdata, stödjer Tiff/XPS |
| [getSheetSet()](#getSheetSet--) | Hämtar bladen som ska renderas. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Hämtar prefixet för css-namnet i svg, standardvärdet är en tom sträng. |
| [getTextCrossType()](#getTextCrossType--) | Hämtar visningstyp för text när textbredden är större än cellbredden. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Hämtar bitdjup som endast tillämpas när sidor sparas i `Tiff`-formatet. |
| [getTiffCompression()](#getTiffCompression--) | Hämtar kompressionstypen som endast tillämpas när sidor sparas i `Tiff`-formatet. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | Hämtar typen av PhotometricInterpretation som endast tillämpas när sidor sparas i `Tiff`-formatet. |
| [getTransparent()](#getTransparent--) | Indikerar om bakgrunden för den genererade bilden ska vara transparent. |
| [getVerticalResolution()](#getVerticalResolution--) | Hämtar den vertikala upplösningen för genererade bilder, i punkter per tum. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Indikerar om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [isOptimized()](#isOptimized--) | Indikerar om utdataelementen ska optimeras. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Indikerar om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Anger diagrammets bildtyp vid konvertering. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [setCssPrefix(String value)](#setCssPrefix-java.lang.String-) | Ställer in prefixet för css-namnet i svg, standardvärdet är en tom sträng. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Ställer in anpassade inställningar under rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Ställer in standardspråk för redigering. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Ställer in önskad bredd och höjd för bilden. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Ställer in önskad bredd och höjd för bilden. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Ställer in typ av teckensnitt som bäddas in i Svg. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Anger filnamnet för den inbäddade bilden i svg. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Inställning för rendering av Emf-metafiler i källfilen. |
| [setFitToViewPort(boolean value)](#setFitToViewPort-boolean-) | Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Ställer in rutnätslinjens färg. |
| [setGridlineType(int value)](#setGridlineType-int-) | Ställer in typ för rutnätslinjer. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Ställer in den horisontella upplösningen för genererade bilder, i punkter per tum. |
| [setImageType(int value)](#setImageType-int-) | Ställer in formatet för de genererade bilderna. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | Om denna egenskap är sann, kommer ett område att skrivas ut, och ingen skala kommer att tillämpas. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Indikerar om utdataelementen ska optimeras. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [setPageCount(int value)](#setPageCount-int-) | Ställer in antalet sidor som ska sparas. |
| [setPageIndex(int value)](#setPageIndex-int-) | Ställer in det 0-baserade indexet för den första sidan som ska sparas. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Styr/indikera framsteg för sid sparningsprocessen. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | Om PrintWithStatusDialog = true, kommer en dialog att visas som visar aktuell utskriftsstatus. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Anger vilka sidor som inte kommer att skrivas ut. |
| [setQuality(int value)](#setQuality-int-) | Ställer in ett värde som bestämmer kvaliteten på de genererade bilderna och som endast tillämpas när sidor sparas i `Jpeg`-format. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Ställer in värdet för ett enskilt alternativ för renderingsalgoritmerna. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Ställer in filformatstypen för utdata, stödjer Tiff/XPS. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Ställer in vilka blad som ska renderas. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Ställer in prefixet för css-namnet i svg, standardvärdet är en tom sträng. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Ställer in visningstyp för text när textbredden är större än cellbredden. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Ställer in bitdjupet som endast tillämpas när sidor sparas i `Tiff`-format. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Ställer in kompressionstypen som endast tillämpas när sidor sparas i `Tiff`-format. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Ställer in typen av PhotometricInterpretation som endast tillämpas när sidor sparas i `Tiff`-format. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indikerar om bakgrunden för den genererade bilden ska vara transparent. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Ställer in den vertikala upplösningen för genererade bilder, i punkter per tum. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SvgImageOptions() {#SvgImageOptions--}
```
public SvgImageOptions()
```


Konstruktor.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll på ett blad att skrivas ut på endast en sida i resultatet. Bredden på papperstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup gäller fortfarande.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


Ange diagrammets bildtyp vid konvertering. standardvärde: PNG.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället renderas Chart och Shape alltid som vektorelement (t.ex. punkt, linje) för renderingskvalitet. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta till true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.

**Remarks**

Standard är true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssPrefix() {#getCssPrefix--}
```
public String getCssPrefix()
```


Hämtar prefixet för css-namnet i svg, standardvärdet är en tom sträng.

**Returns:**
java.lang.String
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Hämtar anpassade inställningar under rendering.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Hämtar standardspråk för redigering.

Se [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Det kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Hämtar typen av teckensnitt som är inbäddad i Svg.

Se [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Standardvärdet är [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE) vilket indikerar att inget teckensnitt kommer att bäddas in i Svg.

**Returns:**
int
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Ange filnamnet för den inbäddade bilden i svg. Detta bör vara en fullständig sökväg med katalog, t.ex. "c:\\\\xpsEmbedded"

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället, ta bort denna egenskap eftersom bilder nu alltid bäddas in i Svg med base64-format. Denna egenskap kommer att tas bort 12 månader senare från och med april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Inställning för rendering av Emf-metafiler i källfilen.

Se [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF-metafiler identifierade som "EMF+ Dual" kan innehålla både EMF+-poster och EMF-poster. Endast en typ av post kan användas för att rendera bilden, antingen bara EMF+-poster eller bara EMF-poster. När [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) är satt, kommer EMF+-poster att analyseras vid rendering till bild, annars analyseras endast EMF-poster. Standardvärdet är [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). För ramverk som är beroende av .NET System.Drawing.Common ignoreras denna inställning.

**Returns:**
int
### getFitToViewPort() {#getFitToViewPort--}
```
public boolean getFitToViewPort()
```


Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Hämtar rutnätslinjens färg.

**Remarks**

Den kommer att ignorera inställningarna för rutnätslinjens färg i källfilen.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Hämtar typ av rutnätslinje.

Se [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Standard är Dotted-typ.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Hämtar den horisontella upplösningen för genererade bilder, i punkter per tum.

**Remarks**

Standardvärdet är 96. Inställning av  och  påverkar bredden och höjden på utdata‑bilden i pixlar.

**Example**

Följande kod sätter upplösningen till 192, bredden och höjden på den genererade bilden blir dubbelt så stor som när upplösningen är kvar på standardvärdet 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Hämtar formatet för de genererade bilderna. standardvärde: PNG.

Se [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Om OnePagePerSheet är true, kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de andra inställningarna i pagesetup kommer fortfarande att tillämpas.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


Om denna egenskap är sann, kommer ett område att skrivas ut, och ingen skala kommer att tillämpas.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.

**Remarks**

Standard är falskt.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Hämtar antalet sidor som ska sparas.

**Remarks**

Standard är System.Int32.MaxValue vilket betyder att alla sidor kommer att renderas.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Hämtar det 0-baserade indexet för den första sidan som ska sparas.

**Remarks**

Standard är 0.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Styr/indikera framsteg för sid sparningsprocessen.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


Om PrintWithStatusDialog = true, kommer en dialog att visas som visar aktuell utskriftsstatus. Annars visas ingen sådan dialog.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


Anger vilka sidor som inte kommer att skrivas ut.

Se [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Hämtar ett värde som bestämmer kvaliteten på de genererade bilderna och som endast tillämpas när sidor sparas i `Jpeg`-formatet. Standardvärdet är 100

**Remarks**

Har effekt endast vid sparande till JPEG. Värdet måste vara mellan 0 och 100. Standardvärdet är 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Denna egenskap kommer att tas bort 12 månader senare, sedan april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar filformatstypen för utdata, stödjer Tiff/XPS

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället för Tiff/Svg, [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); för Xps, använd [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) med [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Denna egenskap kommer att tas bort 12 månader senare, sedan augusti 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Hämtar de blad som ska renderas. Standard är alla synliga blad i arbetsboken: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Inställningen ignoreras när den används i [SheetRender](../../com.aspose.cells/sheetrender)

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


Hämtar prefixet för css-namnet i svg, standardvärdet är en tom sträng.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Denna egenskap kommer att tas bort 12 månader senare, sedan april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Hämtar visningstyp för text när textbredden är större än cellbredden.

Se [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


Hämtar bitdjup som endast tillämpas när sidor sparas i `Tiff`-formatet.

Se [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Har effekt endast vid sparande till TIFF. Om TiffCompression är inställt på CCITT3, CCITT4, kommer detta inte att ha någon effekt, bildens bitdjup för den genererade tiff-filen kommer alltid att vara 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


Hämtar kompressionstypen som endast tillämpas när sidor sparas i `Tiff`-formatet.

Se [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Har effekt endast vid sparande till TIFF. Standardvärdet är Lzw.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


Hämtar typen av PhotometricInterpretation som endast tillämpas när sidor sparas i `Tiff`-formatet.

**Remarks**

Har effekt endast vid sparande till TIFF. Standardvärdet är -1, vilket betyder att ingen PhotometricInterpretation tillämpas.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Indikerar om bakgrunden för den genererade bilden ska vara transparent.

**Remarks**

Standardvärdet är falskt. Det betyder att bakgrunden för de genererade bilderna är vit.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Hämtar den vertikala upplösningen för genererade bilder, i punkter per tum.

**Remarks**

Standardvärdet är 96. Inställning av  och  påverkar bredden och höjden på utdata‑bilden i pixlar.

**Example**

Följande kod sätter upplösningen till 192, bredden och höjden på den genererade bilden blir dubbelt så stor som när upplösningen är kvar på standardvärdet 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Hämtar varningsåteranrop.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


Indikerar om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. Standardvärdet är falskt.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället används inte denna egenskap, vänligen ta bort den. Denna egenskap kommer att tas bort 12 månader senare, sedan augusti 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt.

**Remarks**

Standard är false. Vi kommer först att försöka med standardfonten för Workbook och PdfSaveOption/system för cellfont.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Indikerar om utdataelementen ska optimeras.

**Remarks**

Standardvärdet är falskt. För närvarande, när denna egenskap är satt till true, kommer följande optimeringar att utföras: 1. optimera kantlinjerna. 2. optimera filstorleken vid rendering till Svg-bild.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll på ett blad att skrivas ut på endast en sida i resultatet. Bredden på papperstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup gäller fortfarande.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


Indikerar om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. Standardvärdet är falskt.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället används inte denna egenskap, vänligen ta bort den. Denna egenskap kommer att tas bort 12 månader senare, sedan augusti 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


Ange diagrammets bildtyp vid konvertering. standardvärde: PNG.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället renderas Chart och Shape alltid som vektorelement (t.ex. punkt, linje) för renderingskvalitet. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta till true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.

**Remarks**

Standard är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCssPrefix(String value) {#setCssPrefix-java.lang.String-}
```
public void setCssPrefix(String value)
```


Ställer in prefixet för css-namnet i svg, standardvärdet är en tom sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Ställer in anpassade inställningar under rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Ställer in standardspråk för redigering.

Se [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Det kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Ställer in önskad bredd och höjd för bilden.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) genom att sätta parametern keepAspectRatio till false. Denna egenskap kommer att tas bort 12 månader senare, sedan maj 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredWidth | int | önskad bredd i pixlar |
| desiredHeight | int | önskad höjd i pixlar |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


Ställer in önskad bredd och höjd för bilden.

**Remarks**

Bredden och höjden på den utgående bilden i pixlar kommer endast att baseras på den inställda önskade bredden och höjden. De  och  kommer inte att påverka bredden och höjden på den utgående bilden i detta fall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredWidth | int | önskad bredd i pixlar |
| desiredHeight | int | önskad höjd i pixlar |
| keepAspectRatio | boolean | om bildens ursprungliga bildförhållande ska behållas |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Ställer in typ av teckensnitt som bäddas in i Svg.

Se [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Standardvärdet är [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE) vilket indikerar att inget teckensnitt kommer att bäddas in i Svg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


Ange filnamnet för den inbäddade bilden i svg. Detta bör vara en fullständig sökväg med katalog, t.ex. "c:\\\\xpsEmbedded"

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället, ta bort denna egenskap eftersom bilder nu alltid bäddas in i Svg med base64-format. Denna egenskap kommer att tas bort 12 månader senare från och med april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Inställning för rendering av Emf-metafiler i källfilen.

Se [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF-metafiler identifierade som "EMF+ Dual" kan innehålla både EMF+-poster och EMF-poster. Endast en typ av post kan användas för att rendera bilden, antingen bara EMF+-poster eller bara EMF-poster. När [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) är satt, kommer EMF+-poster att analyseras vid rendering till bild, annars analyseras endast EMF-poster. Standardvärdet är [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). För ramverk som är beroende av .NET System.Drawing.Common ignoreras denna inställning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFitToViewPort(boolean value) {#setFitToViewPort-boolean-}
```
public void setFitToViewPort(boolean value)
```


Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt.

**Remarks**

Standard är false. Vi kommer först att försöka med standardfonten för Workbook och PdfSaveOption/system för cellfont.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Ställer in rutnätslinjens färg.

**Remarks**

Den kommer att ignorera inställningarna för rutnätslinjens färg i källfilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Ställer in typ för rutnätslinjer.

Se [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Standard är Dotted-typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


Ställer in den horisontella upplösningen för genererade bilder, i punkter per tum.

**Remarks**

Standardvärdet är 96. Inställning av  och  påverkar bredden och höjden på utdata‑bilden i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


Ställer in formatet för de genererade bilderna. standardvärde: PNG.

Se [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Om OnePagePerSheet är true, kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de andra inställningarna i pagesetup kommer fortfarande att tillämpas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


Om denna egenskap är sann, kommer ett område att skrivas ut, och ingen skala kommer att tillämpas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


Indikerar om utdataelementen ska optimeras.

**Remarks**

Standardvärdet är falskt. För närvarande, när denna egenskap är satt till true, kommer följande optimeringar att utföras: 1. optimera kantlinjerna. 2. optimera filstorleken vid rendering till Svg-bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.

**Remarks**

Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Ställer in antalet sidor som ska sparas.

**Remarks**

Standard är System.Int32.MaxValue vilket betyder att alla sidor kommer att renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Ställer in det 0-baserade indexet för den första sidan som ska sparas.

**Remarks**

Standard är 0.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Styr/indikera framsteg för sid sparningsprocessen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


Om PrintWithStatusDialog = true, kommer en dialog att visas som visar aktuell utskriftsstatus. Annars visas ingen sådan dialog.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


Anger vilka sidor som inte kommer att skrivas ut.

Se [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


Ställer in ett värde som bestämmer kvaliteten på de genererade bilderna och som endast tillämpas när sidor sparas i `Jpeg`-formatet. Standardvärdet är 100

**Remarks**

Har effekt endast vid sparande till JPEG. Värdet måste vara mellan 0 och 100. Standardvärdet är 100.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


Ställer in värdet för en enskild preferens för renderingsalgoritmerna. Hint-kategorier inkluderar kontroller för renderingskvalitet och den övergripande tid/kvalitet-avvägningen i renderingsprocessen. Se klassen RenderingHints för definitioner av några vanliga nycklar och värden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | java.awt.RenderingHints.Key | nyckeln för hinten som ska ställas in. |
| värde | java.lang.Object | värdet som indikerar preferenser för den angivna hint-kategorin. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


Om denna egenskap är sann, kommer den genererade svg:n att anpassas till visningsporten.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Denna egenskap kommer att tas bort 12 månader senare, sedan april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Ställer in filformatstypen för utdata, stödjer Tiff/XPS.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället för Tiff/Svg, [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); för Xps, använd [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) med [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Denna egenskap kommer att tas bort 12 månader senare, sedan augusti 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Ställer in de blad som ska renderas. Standard är alla synliga blad i arbetsboken: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Inställningen ignoreras när den används i [SheetRender](../../com.aspose.cells/sheetrender)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


Ställer in prefixet för css-namnet i svg, standardvärdet är en tom sträng.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Denna egenskap kommer att tas bort 12 månader senare, sedan april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Ställer in visningstyp för text när textbredden är större än cellbredden.

Se [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


Ställer in bitdjupet som endast tillämpas när sidor sparas i `Tiff`-format.

Se [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Har effekt endast vid sparande till TIFF. Om TiffCompression är inställt på CCITT3, CCITT4, kommer detta inte att ha någon effekt, bildens bitdjup för den genererade tiff-filen kommer alltid att vara 1.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


Ställer in kompressionstypen som endast tillämpas när sidor sparas i `Tiff`-format.

Se [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Har effekt endast vid sparande till TIFF. Standardvärdet är Lzw.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


Ställer in typen av PhotometricInterpretation som endast tillämpas när sidor sparas i `Tiff`-format.

**Remarks**

Har effekt endast vid sparande till TIFF. Standardvärdet är -1, vilket betyder att ingen PhotometricInterpretation tillämpas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indikerar om bakgrunden för den genererade bilden ska vara transparent.

**Remarks**

Standardvärdet är falskt. Det betyder att bakgrunden för de genererade bilderna är vit.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


Ställer in den vertikala upplösningen för genererade bilder, i punkter per tum.

**Remarks**

Standardvärdet är 96. Inställning av  och  påverkar bredden och höjden på utdata‑bilden i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Ställer in varningsåteranrop.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

