---
title: "Workbook"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett rotobjekt för att skapa ett Excel-kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Representerar ett rotobjekt för att skapa ett Excel-kalkylblad.

**Remarks**

Workbook-klassen betecknar ett Excel-kalkylblad. Varje kalkylblad kan innehålla flera arbetsblad. Klassens grundfunktion är att öppna och spara inhemska Excel-filer. Klassen har några avancerade funktioner såsom att kopiera data från andra Workbook‑ar, kombinera två Workbook‑ar, konvertera Excel till PDF, rendera Excel till bild och skydda Excel‑kalkylbladet.

**Example**

Följande exempel laddar en Workbook från en Excel-fil med namnet designer.xls och gör de horisontella och vertikala rullningslisterna osynliga. Det ersätter sedan två strängvärden med respektive ett heltalsvärde och ett strängvärde i kalkylbladet och sparar slutligen arbetsboken som en Excel‑xlsx‑fil.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Workbook()](#Workbook--) | Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(int fileFormatType)](#Workbook-int-) | Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | Initierar en ny tom instans av klassen [Workbook](../../com.aspose.cells/workbook) med alternativ |
| [Workbook(String file)](#Workbook-java.lang.String-) | Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en fil. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en ström. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en fil. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en ström. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Accepterar alla spårade ändringar i arbetsboken. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Lägger till en digital signatur i en OOXML-kalkylbladsfil (Excel2007 och senare). |
| [calculateFormula()](#calculateFormula--) | Beräknar resultatet av formler. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Beräknar resultatet av formler. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Beräknar formler i den här arbetsboken. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Ändrar paletten för kalkylbladet på det angivna indexet. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Stänger sessionen som använder cache för att komma åt data. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Kombinerar ett annat Workbook-objekt. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Kopierar data från ett käll-Workbook-objekt. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Kopierar ett annat Workbook-objekt. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Kopierar temat från en annan arbetsbok. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Skapar inbyggd stil av given typ. |
| [createCellsColor()](#createCellsColor--) | Skapar ett [CellsColor](../../com.aspose.cells/cellscolor)-objekt. |
| [createStyle()](#createStyle--) | Skapar en ny stil. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | Skapar en ny stil. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Anpassar temat. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Exporterar XML-data som är länkad via den angivna XML-kartan. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Exporterar XML-data som är länkad via den angivna XML-kartan. |
| [getAbsolutePath()](#getAbsolutePath--) | Hämtar den absoluta sökvägen för filen. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Hämtar fabriken för att bygga ICellsDataTable från anpassade objekt |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Returnerar färger i paletten för kalkylbladet. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Hämtar listan med [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty)-objekt i arbetsboken. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Hämtar antalet stilar i stilpoolen. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla anpassade dokumentegenskaper i kalkylbladet. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Representerar en Custom XML Data Storage Part (anpassad XML‑data inom ett paket). |
| [getDataConnections()](#getDataConnections--) | Hämtar [ExternalConnection](../../com.aspose.cells/externalconnection)-samlingen. |
| [getDataMashup()](#getDataMashup--) | Hämtar mashup-data. |
| [getDataModel()](#getDataModel--) | Hämtar datamodellen i arbetsboken. |
| [getDataSorter()](#getDataSorter--) | Hämtar ett DataSorter-objekt för att sortera data. |
| [getDefaultStyle()](#getDefaultStyle--) | Hämtar standard [Style](../../com.aspose.cells/style)-objektet i arbetsboken. |
| [getDigitalSignature()](#getDigitalSignature--) | Hämtar digital signatur från fil. |
| [getFileFormat()](#getFileFormat--) | Hämtar filformatet. |
| [getFileName()](#getFileName--) | Hämtar det aktuella filnamnet. |
| [getFonts()](#getFonts--) | Hämtar alla teckensnitt i stilpoolen. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Hämtar avbrottsövervakaren. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Hitta bäst matchande färg i aktuell palett. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Hämtar den namngivna stilen i stilpoolen. |
| [getRibbonXml()](#getRibbonXml--) | Hämtar XML-filen som definierar Ribbon‑UI. |
| [getSettings()](#getSettings--) | Representerar arbetsbokens inställningar. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Hämtar stilen i stilpoolen. |
| [getTheme()](#getTheme--) | Hämtar temats namn. |
| [getThemeColor(int type)](#getThemeColor-int-) | Hämtar temafärgen. |
| [getVbaProject()](#getVbaProject--) | Hämtar [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) i ett kalkylblad. |
| [getWorksheets()](#getWorksheets--) | Hämtar [WorksheetCollection](../../com.aspose.cells/worksheetcollection)-samlingen i kalkylbladet. |
| [hasCustomFunction()](#hasCustomFunction--) | Detekterar om det finns anpassade funktioner som används i den här arbetsboken, till exempel i cellers formel eller i definierade namn... |
| [hasExernalLinks()](#hasExernalLinks--) | Anger om den här arbetsboken innehåller externa länkar till andra datakällor. |
| [hasMacro()](#hasMacro--) | Anger om detta kalkylblad innehåller makro/VBA. |
| [hasRevisions()](#hasRevisions--) | Hämtar om arbetsboken har några spårade ändringar |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Importerar/uppdaterar en XML-datfil i arbetsboken. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Importerar/uppdaterar en XML-datfil i arbetsboken. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Kontrollerar om en färg finns i paletten för kalkylbladet. |
| [isDigitallySigned()](#isDigitallySigned--) | Anger om detta kalkylblad är digitalt signerat. |
| [isLicensed()](#isLicensed--) | Anger om licensen är inställd. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Anger om struktur eller fönster är skyddade med lösenord. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | Slår ihop namngivna format från den andra Excel-filen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Analyserar alla formler som inte har analyserats när de laddades från mallfilen eller sattes i en cell. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Skyddar en arbetsbok. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Skyddar en delad arbetsbok. |
| [refreshAll()](#refreshAll--) | Uppdaterar länkade former, alla pivottabeller och diagram med pivottabellskälla. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data) Andra formler i arbetsboken beräknas inte rekursivt även om de användes av dynamiska matrisformler. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data) |
| [removeDigitalSignature()](#removeDigitalSignature--) | Tar bort digital signatur från detta kalkylblad. |
| [removeExternalLinks()](#removeExternalLinks--) | Tar bort alla externa länkar i arbetsboken. |
| [removeMacro()](#removeMacro--) | Tar bort VBA/makro från detta kalkylblad. |
| [removePersonalInformation()](#removePersonalInformation--) | Tar bort personlig information. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Ta bort alla oanvända format. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Ersätter cellers värden med ny data. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Ersätter cellers värden med ny data. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Ersätter en cells värde med ett nytt dubbelvärde. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Ersätter cellers värden med en dubbelarray. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Ersätter en cells värde med ett nytt heltal. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Ersätter cellers värden med en heltalsarray. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Ersätter en cells värde med en ny sträng. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Ersätter en cells värde med en ny sträng. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Ersätter en cells värde med en ny strängarray. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Spara arbetsboken till strömmen. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Spara arbetsboken till strömmen. |
| [save(String fileName)](#save-java.lang.String-) | Spara arbetsboken till disken. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Sparar arbetsboken till disken. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Sparar arbetsboken till disken. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | Ställer in den absoluta sökvägen för filen. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | Ställer in standard [Style](../../com.aspose.cells/style) objektet för arbetsboken. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Ställer in digital signatur för en kalkylbladsfil (Excel2007 och senare). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Ställ in krypteringsalternativ. |
| [setFileFormat(int value)](#setFileFormat-int-) | Ställer in filformatet. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Ställer in det aktuella filnamnet. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Ställer in avbrottsövervakaren. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | Ställer in XML-filen som definierar Ribbon UI. |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Ställer in temafärgen. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Startar sessionen som använder cache för att komma åt data. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Avskyddar en arbetsbok. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Avskyddar en delad arbetsbok. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Uppdaterar definitionen av anpassade funktioner. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | Om den här arbetsboken innehåller externa länkar till andra datakällor, kommer Aspose.Cells att försöka hämta den senaste datan från de angivna källorna. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Standardfilformatet är Xlsx. Om du vill skapa andra filtyper, använd Workbook(FileFormatType).

**Example**

Följande kod visar hur man använder Workbook‑konstruktorn för att skapa och initiera en ny instans av klassen.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Standardfilformatet är Excel97To2003.

**Example**

Följande kod visar hur man använder Workbook‑konstruktorn för att skapa och initiera en ny instans av klassen med olika filformat.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). Det nya filformatet. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


Initierar en ny tom instans av klassen [Workbook](../../com.aspose.cells/workbook) med alternativ

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Alternativen. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fil | java.lang.String | Filnamnet. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Strömmen. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fil | java.lang.String | Filnamnet. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Laddningsalternativen |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Initierar en ny instans av klassen [Workbook](../../com.aspose.cells/workbook) och öppnar en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Strömmen. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Laddningsalternativen |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Accepterar alla spårade ändringar i arbetsboken.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Lägger till en digital signatur i en OOXML-kalkylbladsfil (Excel2007 och senare).

**Remarks**

Stöder endast att lägga till Xmldsig digital signatur till en OOXML‑kalkylbladsfil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Beräknar resultatet av formler.

**Remarks**

För alla stödda formler, se listan på https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Beräknar resultatet av formler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ignoreError | boolean | Anger om fel vid beräkning av formler ska döljas. Felet kan vara en funktion som inte stöds, externa länkar osv. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Beräknar formler i den här arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för beräkning |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Ändrar paletten för kalkylbladet på det angivna indexet.

**Remarks**

Paletten har 56 poster, var och en representerad av ett RGB‑värde.

Om du anger en färg som inte finns i paletten kommer den inte att ha någon effekt.

Så om du vill ange en anpassad färg, ändra paletten först.

Följande är den standardfärgpaletten.

| Color | Röd | Grön | Blå |
| ------- | --- | ----- | ---- |
| Svart | 0 | 0 | 0 |
| Vit | 255 | 255 | 255 |
| Röd | 255 | 0 | 0 |
| Lime | 0 | 255 | 0 |
| Blå | 0 | 0 | 255 |
| Gul | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Cyan | 0 | 255 | 255 |
| Mörkröd | 128 | 0 | 0 |
| Grön | 0 | 128 | 0 |
| Marinblå | 0 | 0 | 128 |
| Oliv | 128 | 128 | 0 |
| Lila | 128 | 0 | 128 |
| Blågrön | 0 | 128 | 128 |
| Silver | 192 | 192 | 192 |
| Grå | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Färg19 | 255 | 255 | 204 |
| Färg20 | 204 | 255 | 255 |
| Färg21 | 102 | 0 | 102 |
| Färg22 | 255 | 128 | 128 |
| Färg23 | 0 | 102 | 204 |
| Färg24 | 204 | 204 | 255 |
| Färg25 | 0 | 0 | 128 |
| Färg26 | 255 | 0 | 255 |
| Färg27 | 255 | 255 | 0 |
| Färg28 | 0 | 255 | 255 |
| Färg29 | 128 | 0 | 128 |
| Färg30 | 128 | 0 | 0 |
| Färg31 | 0 | 128 | 128 |
| Färg32 | 0 | 0 | 255 |
| Färg33 | 0 | 204 | 255 |
| Färg34 | 204 | 255 | 255 |
| Färg35 | 204 | 255 | 204 |
| Färg36 | 255 | 255 | 153 |
| Färg37 | 153 | 204 | 255 |
| Färg38 | 255 | 153 | 204 |
| Färg39 | 204 | 153 | 255 |
| Färg40 | 255 | 204 | 153 |
| Färg41 | 51 | 102 | 255 |
| Color42 | 51 | 204 | 204 |
| Color43 | 153 | 204 | 0 |
| Color44 | 255 | 204 | 0 |
| Color45 | 255 | 153 | 0 |
| Color46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Färgsstruktur. |
| index | int | Palettindex, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Stänger sessionen som använder cache för att komma åt data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). alternativ för dataåtkomst |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Kombinerar ett annat Workbook-objekt.

**Remarks**

Sammanfoga Excel, ODS, CSV och andra filer till en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | En annan Workbook-objekt. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Kopierar data från ett käll-Workbook-objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Käll Workbook-objekt. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Kopierar ett annat Workbook-objekt.

**Remarks**

Det är mycket enkelt att klona en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Käll Workbook-objekt. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Alternativen för att kopiera annan workbook. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Kopierar temat från en annan arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Käll workbook. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Skapar inbyggd stil av given typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). Den inbyggda stiltypen. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Skapar ett [CellsColor](../../com.aspose.cells/cellscolor)-objekt.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Skapar en ny stil.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


Skapar en ny stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cloneDefaultStyle | boolean | Anger om standardstilen klonas |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Anpassar temat.

**Remarks**

Längden på färgerna bör vara 12.

| Array-index | Tematyp |
| ----------- | ------------------ |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Hyperlänk |
| 11 | Följd hyperlänk |

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| themeName | java.lang.String | Temanamnet |
| colors | [Color\[\]](../../com.aspose.cells/color) | Temafärgerna |

### dispose() {#dispose--}
```
public void dispose()
```


Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser.

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Exporterar XML-data som är länkad via den angivna XML-kartan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mapName | java.lang.String | namnet på XML-kartan som ska exporteras |
| stream | java.io.OutputStream | exportströmmen |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Exporterar XML-data som är länkad via den angivna XML-kartan.

**Example**

Följande kod exporterade data som länkas av den första XmlMap.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mapName | java.lang.String | namnet på XML-kartan som ska exporteras |
| sökväg | java.lang.String | exportvägen |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


Hämtar den absoluta sökvägen för filen.

**Remarks**

Används endast för externa länkar.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet.

**Remarks**

En ny egenskap kan inte läggas till i listan över inbyggda dokumentegenskaper. Du kan bara hämta en inbyggd egenskap och ändra dess värde. Följande är listan över namn på inbyggda egenskaper:

Titel

Ämne

Författare

Nyckelord

Kommentarer

Mall

Senaste författare

Revisionsnummer

Programnamn

Senaste utskriftsdatum

Skapandedatum

Senaste sparningstid

Total redigeringstid

Antal sidor

Antal ord

Antal tecken

Säkerhet

Kategori

Format

Ansvarig

Företag

Antal byte

Antal rader

Antal stycken

Antal bilder

Antal anteckningar

Antal dolda bilder

Antal multimedieklipp

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Hämtar fabriken för att bygga ICellsDataTable från anpassade objekt

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Returnerar färger i paletten för kalkylbladet.

**Remarks**

Paletten har 56 poster, var och en representerad av ett RGB‑värde.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Hämtar listan med [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty)-objekt i arbetsboken.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Hämtar antalet stilar i stilpoolen.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla anpassade dokumentegenskaper i kalkylbladet.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Representerar en Custom XML Data Storage Part (anpassad XML‑data inom ett paket).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


Hämtar [ExternalConnection](../../com.aspose.cells/externalconnection)-samlingen.

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Hämtar mashup-data.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


Hämtar datamodellen i arbetsboken.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Hämtar ett DataSorter-objekt för att sortera data.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


Hämtar standard [Style](../../com.aspose.cells/style)-objektet i arbetsboken.

**Remarks**

Egenskapen DefaultStyle är användbar för att implementera en Stil för hela Arbetsboken.

**Example**

Följande kod skapar och instansierar en ny Arbetsbok och sätter en standard [Style](../../com.aspose.cells/style) på den.

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Hämtar digital signatur från fil.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Hämtar filformatet.

Se [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


Hämtar det aktuella filnamnet.

**Remarks**

Om filen öppnas via ström och det finns externa formelreferenser, ange filnamnet.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Hämtar alla teckensnitt i stilpoolen.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Hämtar avbrottsövervakaren.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Hitta bäst matchande färg i aktuell palett.

**Remarks**

Det finns bara 56 färger i färgpaletten i Excel 97-2003. Om färgen inte finns i paletten, kommer en liknande färg att sättas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Rå färg. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Hämtar den namngivna stilen i stilpoolen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | namnet på stilen |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


Hämtar XML-filen som definierar Ribbon‑UI.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Representerar arbetsbokens inställningar.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Hämtar stilen i stilpoolen. Alla stilar i arbetsboken samlas i en pool. Det finns bara ett enkelt referensindex i cellerna.

**Remarks**

Om den returnerade stilen ändras, kommer stilen för alla celler (som refererar till denna stil) att ändras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Hämtar temats namn.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Hämtar temafärgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Temafärgstypen. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Hämtar [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) i ett kalkylblad.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Hämtar [WorksheetCollection](../../com.aspose.cells/worksheetcollection)-samlingen i kalkylbladet.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Detekterar om det finns anpassade funktioner som används i den här arbetsboken, till exempel i cellers formel eller i definierade namn...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Anger om den här arbetsboken innehåller externa länkar till andra datakällor.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället ExternalLinkCollection.Count för att kontrollera om det finns externa länkar i denna arbetsbok. Denna metod kommer att tas bort 12 månader senare sedan december 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean - Om denna arbetsbok innehåller externa länkar till andra datakällor.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Anger om detta kalkylblad innehåller makro/VBA.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Hämtar om arbetsboken har några spårade ändringar

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Importerar/uppdaterar en XML-datfil i arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | xml‑filströmmen. |
| sheetName | java.lang.String | namnet på destinationsbladet. |
| rad | int | destinationsraden. |
| kol | int | destinationskolumnen. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Importerar/uppdaterar en XML-datfil i arbetsboken.

**Example**

Följande kod importerar xml‑data till kalkylbladet 'Sheet 1' i cell A1.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| url | java.lang.String | url‑/sökvägen till xml‑filen. |
| sheetName | java.lang.String | namnet på destinationsbladet. |
| rad | int | destinationsraden |
| kol | int | destinationskolumnen |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Kontrollerar om en färg finns i paletten för kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Färgsstruktur. |

**Returns:**
boolean - Returnerar true om denna färg finns i paletten. Annars returneras false.
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Anger om detta kalkylblad är digitalt signerat.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Anger om licensen är inställd.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Anger om struktur eller fönster är skyddade med lösenord.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


Slår ihop namngivna format från den andra Excel-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Den andra filen |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Analyserar alla formler som inte har analyserats när de laddades från mallfilen eller sattes i en cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ignoreError | boolean | Om fel ska ignoreras för ogiltig formel. För en ogiltig formel, om fel ignoreras så kommer denna formel att hoppas över och processen fortsätter att tolka andra formler, annars kastas ett undantag. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Skyddar en arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Skyddstyp. |
| lösenord | java.lang.String | Lösenord för att skydda arbetsboken. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Skyddar en delad arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | Lösenord för att skydda arbetsboken. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Uppdaterar länkade former, alla pivottabeller och diagram med pivottabellskälla.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data) Andra formler i arbetsboken beräknas inte rekursivt även om de användes av dynamiska matrisformler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| beräkna | boolean | Om cellvärden beräknas och uppdateras för dessa dynamiska matrisformler |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data)

**Remarks**

Av prestandaskäl uppdaterar vi inte alla dynamiska matrisformler automatiskt när formeln själv eller de data den refererar till ändras. Därför måste användaren anropa den här metoden manuellt efter de operationer som kan påverka dynamiska matrisformler, såsom import/inställning av cellvärden, infogning/borttagning av rader/kolumner/områden, ...etc.

För de flesta formler med funktioner kräver beräkning av spill‑området också beräkning av formeln, så i allmänhet föredras värdet true för flaggan "calculate". Om formeln är enkel, såsom en områdesreferens eller matris (till exempel "=C1:E5", "=\\{1,2;3,4\\}", …), enkel funktion på ett område eller en matris (till exempel "=ABS(C1:E5)", "=1+\\{1,2;3,4\\}", …), och alla formler kommer att beräknas senare (till exempel via [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-)), kan användning av värdet false för flaggan "calculate" undvika duplicerad beräkning till fördel för prestandan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| beräkna | boolean | Om cellvärden beräknas och uppdateras för dessa dynamiska matrisformler |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativen för att beräkna formler |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Tar bort digital signatur från detta kalkylblad.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Tar bort alla externa länkar i arbetsboken.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden ExternalLinkCollection.Clear(). Denna metod kommer att tas bort 12 månader senare, sedan december 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Tar bort VBA/makro från detta kalkylblad.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Tar bort personlig information.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Ta bort alla oanvända format.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Ersätter cellers värden med ny data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| boolValue | boolean | Det booleska värdet som ska ersättas. |
| newValue | java.lang.Object | Nytt värde. Kan vara en sträng, heltal, dubbel eller DateTime‑värde. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Ersätter cellers värden med ny data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intValue | int | Det heltalsvärdet som ska ersättas. |
| newValue | java.lang.Object | Nytt värde. Kan vara en sträng, heltal, dubbel eller DateTime‑värde. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Ersätter en cells värde med ett nytt dubbelvärde.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValue | double | Dubbelvärde att ersätta |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Ersätter cellers värden med en dubbelarray.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValues | double[] | Dubbelarray att ersätta |
| isVertical | boolean | Sant - Vertikal, Falskt - Horisontell |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Ersätter en cells värde med ett nytt heltal.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValue | int | Heltalsvärde att ersätta |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Ersätter cellers värden med en heltalsarray.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValues | int[] | Heltalsarray att ersätta |
| isVertical | boolean | Sant - Vertikal, Falskt - Horisontell |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Ersätter en cells värde med en ny sträng.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValue | java.lang.String | Strängvärde att ersätta |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Ersätter en cells värde med en ny sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValue | java.lang.String | Strängvärde att ersätta |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Ersättningsalternativen |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Ersätter en cells värde med en ny strängarray.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValues | java.lang.String[] | Strängarray att ersätta |
| isVertical | boolean | Sant - Vertikal, Falskt - Horisontell |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Spara arbetsboken till strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Filströmmen. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Sparaalternativen. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Spara arbetsboken till strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Filströmmen. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Spara filformatstypen. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Spara arbetsboken till disken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Sparar arbetsboken till disken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamnet. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Sparaalternativen. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Sparar arbetsboken till disken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamnet. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Spara formattyp. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


Ställer in den absoluta sökvägen för filen.

**Remarks**

Används endast för externa länkar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


Ställer in standard [Style](../../com.aspose.cells/style) objektet för arbetsboken.

**Remarks**

Egenskapen DefaultStyle är användbar för att implementera en Stil för hela Arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Ställer in digital signatur för en kalkylbladsfil (Excel2007 och senare).

**Remarks**

Stöder endast att lägga till Xmldsig Digital Signature

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Ställ in krypteringsalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). Krypteringstypen. |
| keyLength | int | Nyckellängden. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


Ställer in filformatet.

Se [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


Ställer in det aktuella filnamnet.

**Remarks**

Om filen öppnas via ström och det finns externa formelreferenser, ange filnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Ställer in avbrottsövervakaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


Ställer in XML-filen som definierar Ribbon UI.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Ställer in temafärgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Temafärgstypen. |
| color | [Color](../../com.aspose.cells/color) | temafärgen |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Startar sessionen som använder cache för att komma åt data.

**Remarks**

Om cachen för den specificerade dataåtkomsten kräver att vissa datamodeller i kalkylbladet är "read-only", kommer motsvarande datamodeller i varje kalkylblad i den här arbetsboken att betraktas som "read-only" och användaren bör inte ändra någon av dem.

Efter att ha avslutat åtkomsten till data, bör [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) anropas med samma alternativ för att rensa alla cachar och återställa normalt åtkomstläge.



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). alternativ för dataåtkomst |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Avskyddar en arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | Lösenord för att ta bort skyddet från arbetsboken. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Avskyddar en delad arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | Lösenord för att ta bort skyddet från arbetsboken. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


Uppdaterar definitionen av anpassade funktioner.

**Remarks**

Denna metod kan användas för vissa speciella scenarier. Till exempel, om användaren behöver vissa parametrar för anpassade funktioner beräknas i array‑läge, kan användaren tillhandahålla sin egen definition med den implementerade [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) för dessa funktioner. Efter att formeldata har uppdaterats kommer de angivna parametrarna att beräknas i array‑läge automatiskt när motsvarande anpassade funktioner beräknas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | Specialdefinition av anpassade funktioner för användarens speciella krav. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


Om den här arbetsboken innehåller externa länkar till andra datakällor, kommer Aspose.Cells att försöka hämta den senaste datan från de angivna källorna.

**Remarks**

Om motsvarande extern länk inte kan hittas för en arbetsbok, kommer den arbetsboken att ignoreras. Så när du senare anger en formel med en ny extern länk som du avser att länka den ignorerade arbetsboken till, kan länken inte utföras förrän du anropar den här metoden igen med de arbetsböckerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | Arbetsböcker som kommer att användas för att uppdatera data för externa länkar som refereras av denna arbetsbok. Matchningen av dessa arbetsböcker med externa länkar bestäms av [getFileName()](../../com.aspose.cells/workbook\#getFileName--) och [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Så se till att [getFileName()](../../com.aspose.cells/workbook\#getFileName--) har angetts med rätt värde för varje arbetsbok så att de kan länkas till motsvarande externa länk. |

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

