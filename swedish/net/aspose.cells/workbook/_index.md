---
title: Workbook
second_title: Aspose.Cells för .NET API-referens
description: Representerar ett rotobjekt för att skapa ett Excel-kalkylblad.
type: docs
weight: 6480
url: /sv/net/aspose.cells/workbook/
---
## Workbook class

Representerar ett rotobjekt för att skapa ett Excel-kalkylblad.

```csharp
public class Workbook : IDisposable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Workbook](workbook#constructor)() | Initierar en ny instans av[`Workbook`](../workbook) class. |
| [Workbook](workbook#constructor_1)(FileFormatType) | Initierar en ny instans av[`Workbook`](../workbook) class. |
| [Workbook](workbook#constructor_2)(Stream) | Initierar en ny instans av[`Workbook`](../workbook) klass och öppna en stream. |
| [Workbook](workbook#constructor_4)(string) | Initierar en ny instans av[`Workbook`](../workbook) klass och öppna en fil. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | Initierar en ny instans av[`Workbook`](../workbook) klass och öppen ström. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | Initierar en ny instans av[`Workbook`](../workbook) klass och öppna en fil. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | Hämtar och ställer in den absoluta sökvägen för filen. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | Returnerar en[`DocumentProperty`](../../aspose.cells.properties/documentproperty)samling som representerar alla inbyggda dokumentegenskaper i kalkylarket. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | Får fabriken för att bygga ICellsDataTable från anpassade objekt |
| [Colors](../../aspose.cells/workbook/colors) { get; } | Returnerar färger i paletten för kalkylarket. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | Hämtar listan över[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) objekt i arbetsboken. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | Får antalet stilar i stilpoolen. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | Returnerar en[`DocumentProperty`](../../aspose.cells.properties/documentproperty) samling som representerar alla anpassade dokumentegenskaper i kalkylarket. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | Representerar en anpassad XML-datalagringsdel (anpassad XML-data i ett paket). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | Får[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) samling. |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | Får mashup-data. |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | Hämtar ett DataSorter-objekt för att sortera data. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | Hämtar eller ställer in standard[`Style`](../style) objekt för arbetsboken. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | Hämtar och ställer in filformatet. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | Hämtar och ställer in det aktuella filnamnet. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | Indikerar om detta kalkylblad innehåller makro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | Hämtar om arbetsboken har några spårade ändringar |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | Hämtar och ställer in avbrottsmonitorn. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | Indikerar om detta kalkylblad är digitalt signerat. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | Indikerar om licensen är inställd. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | Indikerar om strukturen eller fönstret är skyddat med lösenord. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | Hämtar och ställer in XML-filen som definierar Ribbon UI. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | Representerar arbetsboksinställningarna. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | Hämtar temanamnet. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | Får[`VbaProject`](./vbaproject) i ett kalkylblad. |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | Får[`WorksheetCollection`](../worksheetcollection) samling i kalkylarket. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | Accepterar alla spårade ändringar i arbetsboken. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | Lägger till digital signatur till en OOXML-kalkylarksfil (Excel2007 och senare). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | Beräknar resultatet av formler. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | Beräknar resultatet av formler. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | Beräknar formler i denna arbetsbok. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | Ändrar paletten för kalkylarket i det angivna indexet. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | Stänger sessionen som använder cachar för att komma åt data. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | Kombinerar ett annat arbetsboksobjekt. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | Kopierar data från ett källarbetsboksobjekt. |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | Kopierar data från ett källarbetsboksobjekt. |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | Kopierar temat från en annan arbetsbok. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | Skapar inbyggd stil efter given typ. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | Skapar en[`CellsColor`](../cellscolor) objekt. |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | Skapar en ny stil. |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | Anpassar temat. |
| [Dispose](../../aspose.cells/workbook/dispose)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | Exportera XML-data. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | Exportera XML-data länkade av den angivna XML-kartan. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | Får digital signatur från filen. |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | Får alla typsnitt i stilpoolen. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | Hitta bäst matchande färg i aktuell palett. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | Hämtar den namngivna stilen i stilpoolen. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | Hämtar stilen i stilpoolen. Alla stilar i arbetsboken kommer att samlas i en pool. Det finns bara ett enkelt referensindex i cellerna. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | Får temafärg. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | Importerar/uppdaterar en XML-datafil till arbetsboken. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | Importerar/uppdaterar en XML-datafil till arbetsboken. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | Kontrollerar om en färg finns i paletten för kalkylarket. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | Analyserar alla formler som inte har analyserats när de laddades från mallfilen eller sattes till en cell. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | Skyddar en arbetsbok. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | Skyddar en delad arbetsbok. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | Uppdaterar dynamiska matrisformler (spill in i ett nytt intervall av närliggande celler enligt aktuella data) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | Tar bort digital signatur från det här kalkylarket. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | Tar bort VBA/makro från detta kalkylblad. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | Tar bort personlig information. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | Ta bort alla oanvända stilar. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | Ersätter cellernas värden med nya data. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | Ersätter cellernas värden med nya data. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | Ersätter cellernas värden med data från enDataTable . |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | Ersätter en cells värde med en ny dubbel. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | Ersätter en cells värde med ett nytt heltal. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | Ersätter en cells värde med en ny sträng. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | Ersätter cellernas värden med en dubbel array. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | Ersätter cellvärden med en heltalsmatris. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | Ersätter en cells värde med en ny sträng. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | Ersätter en cells värde med en ny strängmatris. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | Spara arbetsboken på disken. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | Sparar arbetsboken i strömmen. |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | Sparar arbetsboken i strömmen. |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | Sparar arbetsboken på disken. |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | Sparar arbetsboken på disken. |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Skapar resultatkalkylarket och överför det till klienten och öppna det sedan i webbläsaren eller MS Workbook. |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Skapar resultatkalkylarket och överför det till klienten och öppna det sedan i webbläsaren eller MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | Sparar Excel-fil till ett MemoryStream-objekt och returnerar den. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | Ställer in digital signatur till en kalkylarksfil (Excel2007 och senare). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | Ställ in krypteringsalternativ. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | Ställer in temat color |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | Startar sessionen som använder cachar för att komma åt data. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | Tar bort skyddet av en arbetsbok. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | Tar bort skyddet av en delad arbetsbok. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | Om den här arbetsboken innehåller externa länkar till andra datakällor, kommer Aspose.Cells att försöka hämta de senaste uppgifterna. |

### Anmärkningar

Klassen Workbook betecknar ett Excel-kalkylblad. Varje kalkylblad kan innehålla flera kalkylblad. Klassens grundläggande funktion är att öppna och spara inbyggda excel-filer. Klassen har några avancerade funktioner som att kopiera data från andra arbetsböcker, kombinera två arbetsböcker och skydda Excel-kalkylarket.

### Exempel

Följande exempel läser in en arbetsbok från en fil med namnet designer.xls och gör de horisontella och vertikala rullningslisterna osynliga för arbetsboken. Den ersätter sedan två strängvärden med ett heltalsvärde respektive ett strängvärde i kalkylarket och skickar slutligen den uppdaterade filen till klientens webbläsare.

```csharp
[C#]

//Öppna en designerfil
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//Sätt rullningslister
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//Ersätt platshållarsträngen med nya värden
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Öppna en designerfil
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Ställ in rullningslister
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Ersätt platshållarsträngen med nya värden
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
