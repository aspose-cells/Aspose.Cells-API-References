---
title: "CellsHelper"
second_title: "Aspose.Cells för Java API-referens"
description: "Tillhandahåller hjälpfunktioner."
type: docs
url: /sv/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

Tillhandahåller hjälpfunktioner.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Lägg till tilläggsfunktion. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Hämtar cellnamnet enligt dess rad- och kolumnindex. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Hämtar cellens rad- och kolumnindex enligt dess namn. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Hämtar kolumnnamn enligt kolumnindex. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Hämtar kolumnindex enligt kolumnnamn. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Konverterar A1-formeln för cellen till r1c1-formeln. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Konverterar r1c1-formeln för cellen till A1-formeln. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Kontrollerar angivet bladnamn och skapar ett giltigt vid behov. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Kontrollerar angivet bladnamn och skapar ett giltigt vid behov. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Hämtar den alternativa startvägen som refereras av vissa externa formelreferenser. |
| [getCacheFolder()](#getCacheFolder--) | Hämtar mappen för temporära filer som kan användas som datacache. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Hämtar fabriken för att skapa instanser med speciell implementation. |
| [getDPI()](#getDPI--) | Hämtar maskinens DPI. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Konvertera dubbelvärdet till datum-tidsvärdet. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Konvertera datum-tiden till dubbelvärde. |
| [getLibraryPath()](#getLibraryPath--) | Hämtar biblioteksökvägen som refereras av vissa externa formelreferenser. |
| [getSignificantDigits()](#getSignificantDigits--) | Hämtar antalet signifikanta siffror. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Hämtar standardtypen för signifikanta siffror vid utskrift av numeriska värden. |
| [getStartupPath()](#getStartupPath--) | Hämtar startvägen som refereras av vissa externa formelreferenser. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Hämta bredden på texten i enheten punkter. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Hämtar alla använda färger i arbetsboken. |
| [getVersion()](#getVersion--) | Hämta utgivningsversionen. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Vänligen sätt denna egenskap till True när du kör på en molnplattform, såsom: Azure, AWSLambda, etc, |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Slår samman några stora xls-filer till en xls-fil. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Anger om bladnamnet ska omges av enkla citattecken. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Hämtar radnamn enligt radindex. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Hämtar radindex enligt radnamn. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Ställer in den alternativa startvägen, som refereras till av vissa externa formelreferenser. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Ställer in mappen för temporära filer som kan användas som datacache. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Vänligen sätt denna egenskap till True när du kör på en molnplattform, såsom: Azure, AWSLambda, etc, |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Ställer in fabriken för att skapa instanser med specialimplementation. |
| [setDPI(double value)](#setDPI-double-) | Hämtar maskinens DPI. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Ställer in biblioteksökvägen som refereras till av vissa externa formelreferenser. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Ställer in antalet signifikanta siffror. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Ställer in standardtypen för signifikanta siffror vid utskrift av numeriska värden. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Ställer in startvägen, som refereras till av vissa externa formelreferenser. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


Lägg till tilläggsfunktion.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället WorksheetCollection.RegisterAddInFunction()‑metoderna. Denna metod kommer att tas bort 12 månader senare från och med januari 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| funktion | java.lang.String | Funktionens namn. |
| minCountOfParameters | int | Minsta antal parametrar som denna funktion kräver |
| maxCountOfParameters | int | Maximalt antal parametrar som denna funktion tillåter. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). Den förväntade parametertypen för funktionen |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). Funktionsvärdetypen. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Hämtar cellnamnet enligt dess rad- och kolumnindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |

**Returns:**
java.lang.String - Cellens namn.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


Hämtar cellens rad- och kolumnindex enligt dess namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellens namn |

**Returns:**
int[] - [0] är radindex och [1] är kolumnindex.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Hämtar kolumnnamn enligt kolumnindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |

**Returns:**
java.lang.String - Kolumnens namn.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Hämtar kolumnindex enligt kolumnnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnName | java.lang.String | Kolumnnamn. |

**Returns:**
int - Kolumnindex.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


Konverterar A1-formeln för cellen till r1c1-formeln.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Worksheet.ConvertFormulaReferenceStyle()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | A1-formeln. |
| rad | int | Radindex för cellen. |
| kolumn | int | Kolumnindex för cellen. |

**Returns:**
java.lang.String - R1C1-formeln.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


Konverterar r1c1-formeln för cellen till A1-formeln.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Worksheet.ConvertFormulaReferenceStyle()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| r1c1Formula | java.lang.String | r1c1-formeln. |
| rad | int | Radindex för cellen. |
| kolumn | int | Kolumnindex för cellen. |

**Returns:**
java.lang.String - A1-formeln.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn, returneras det. Annars trunkeras strängen om längden överskrider gränsen och ogiltiga tecken ersätts med ' ', sedan returneras det återuppbyggda strängvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nameProposal | java.lang.String | bladnamn att använda |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn, returneras det. Annars trunkeras strängen om längden överskrider gränsen och ogiltiga tecken ersätts med angivet tecken, sedan returneras det återuppbyggda strängvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nameProposal | java.lang.String | bladnamn att använda |
| replaceChar | char | tecken som kommer att användas för att ersätta ogiltiga tecken i angivet bladnamn |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


Hämtar den alternativa startvägen som refereras av vissa externa formelreferenser.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


Hämtar mappen för temporära filer som kan användas som datacache.

**Remarks**

Cache-filer används i allmänhet för vissa funktioner för minnesprestanda, såsom att spara stora datamängder till xls-fil, eller att använda minnesläge med filcache för cellmodellen.

**Returns:**
java.lang.String - Mapp för cache-filer som har angetts. Om den inte har angetts returneras null och systemets temporära sökväg används vid behov.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


Hämtar fabriken för att skapa instanser med speciell implementation.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Hämtar maskinens DPI.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


Konvertera dubbelvärdet till datum-tidsvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| doubleValue | double | Dubbeltvärdet. |
| date1904 | boolean | 1904-datumsystem. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


Konvertera datum-tiden till dubbelvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Datum och tid. |
| date1904 | boolean | 1904-datumsystem. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


Hämtar biblioteksökvägen som refereras av vissa externa formelreferenser.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


Hämtar antalet signifikanta siffror. Standardvärdet är 17.

**Remarks**

Kan bara vara 15 eller 17 nu. OBS: Denna medlem är nu föråldrad. Använd istället [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Denna egenskap kommer att tas bort 12 månader senare från och med juni 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


Hämtar standardtypen för signifikanta siffror vid utskrift av numeriska värden. Standardvärdet är [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Se [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


Hämtar startvägen som refereras av vissa externa formelreferenser.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


Hämta bredden på texten i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Texten. |
| font | [Font](../../com.aspose.cells/font) | Typsnittet för texten. |
| skalning | double | Skalning av texten. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


Hämtar alla använda färger i arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Arbetsboksobjektet. |

**Returns:**
com.aspose.cells.Color[] - De använda färgerna.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Hämta utgivningsversionen.

**Returns:**
java.lang.String - Versionsnumret.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


Vänligen sätt denna egenskap till True när du kör på en molnplattform, såsom: Azure, AWSLambda, etc,

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


Slår samman några stora xls-filer till en xls-fil.

**Remarks**

Denna metod stöder endast sammanslagning av data, stil och formler till den nya filen. Den cachade filen används för att lagra viss temporär data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filer | java.lang.String[] | Filerna. |
| cachedFile | java.lang.String | Den cachade filen. |
| destFile | java.lang.String | Destinationsfilen. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


Anger om bladnamnet ska omges av enkla citattecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Namnet på bladet |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


Hämtar radnamn enligt radindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |

**Returns:**
java.lang.String - Radens namn.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


Hämtar radindex enligt radnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowName | java.lang.String | Radnamn. |

**Returns:**
int - Radindex.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


Ställer in den alternativa startvägen, som refereras till av vissa externa formelreferenser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


Ställer in mappen för temporära filer som kan användas som datacache.

**Remarks**

Cache-filer används i allmänhet för vissa funktioner för minnesprestanda, såsom att spara stora datamängder till xls-fil, eller att använda minnesläge med filcache för cellmodellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cache | java.lang.String | Mapp för temporära filer som kan användas som datacache. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


Vänligen sätt denna egenskap till True när du kör på en molnplattform, såsom: Azure, AWSLambda, etc,

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


Ställer in fabriken för att skapa instanser med specialimplementation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Hämtar maskinens DPI.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


Ställer in biblioteksökvägen som refereras till av vissa externa formelreferenser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


Ställer in antalet signifikanta siffror. Standardvärdet är 17.

**Remarks**

Kan bara vara 15 eller 17 nu. OBS: Denna medlem är nu föråldrad. Använd istället [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Denna egenskap kommer att tas bort 12 månader senare från och med juni 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


Ställer in standardtypen av signifikanta siffror för utskrift av numeriska värden. Standardvärdet är [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Se [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


Ställer in startvägen, som refereras till av vissa externa formelreferenser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

