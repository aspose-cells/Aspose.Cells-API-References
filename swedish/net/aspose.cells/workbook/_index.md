---
title: "Klass Workbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Workbook-klass. Representerar ett rotobjekt för att skapa ett Excel-kalkylblad"
type: docs
url: /sv/net/aspose.cells/workbook/
---
## Workbook class

Representerar ett rotobjekt för att skapa ett Excel-kalkylblad.

```csharp
public class Workbook : IDisposable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Workbook](workbook/#constructor)() | Initierar en ny instans av `Workbook`-klassen. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | Initierar en ny instans av `Workbook`-klassen. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | Initierar en ny tom instans av `Workbook`-klassen med alternativ |
| [Workbook](workbook/#constructor_3)(Stream) | Initierar en ny instans av `Workbook`-klassen och öppnar en ström. |
| [Workbook](workbook/#constructor_5)(string) | Initierar en ny instans av `Workbook`-klassen och öppnar en fil. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | Initierar en ny instans av `Workbook`-klassen och öppnar en ström. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | Initierar en ny instans av `Workbook`-klassen och öppnar en fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Hämtar och anger den absoluta sökvägen för filen. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Returnerar en [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) samling som representerar alla inbyggda dokumentegenskaper i kalkylarket. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Hämtar fabriken för att bygga ICellsDataTable från anpassade objekt |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Returnerar färger i paletten för kalkylbladet. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Hämtar listan med [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) objekt i arbetsboken. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Hämtar antalet stilar i stilpoolen. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Returnerar en [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) samling som representerar alla anpassade dokumentegenskaper i kalkylarket. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Representerar en anpassad XML‑databasdel (anpassad XML‑data inom ett paket). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | Hämtar [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/) samlingen. |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Hämtar mashup-data. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Hämtar datamodellen i arbetsboken. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Hämtar ett DataSorter-objekt för att sortera data. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Hämtar eller anger standard [`Style`](../style/) objektet för arbetsboken. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Hämtar och anger filformatet. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Hämtar och anger det aktuella filnamnet. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Detekterar om det finns anpassade funktioner som används i den här arbetsboken, till exempel i cellers formel eller i definierade namn... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Anger om detta kalkylblad innehåller makro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Hämtar om arbetsboken har några spårade ändringar |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsövervakaren. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Anger om detta kalkylblad är digitalt signerat. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Anger om licensen är inställd. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Anger om struktur eller fönster är skyddade med lösenord. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Hämtar och anger XML-filen som definierar Ribbon‑UI. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Representerar arbetsbokens inställningar. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Hämtar temats namn. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Hämtar [`VbaProject`](./vbaproject/) i ett kalkylblad. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Hämtar [`WorksheetCollection`](../worksheetcollection/) samlingen i kalkylbladet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Accepterar alla spårade ändringar i arbetsboken. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | Lägger till digital signatur i en OOXML-kalkylbladsfil (Excel2007 och senare). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Beräknar resultatet av formler. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Beräknar resultatet av formler. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Beräknar formler i den här arbetsboken. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Ändrar paletten för kalkylbladet på angivet index. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Stänger sessionen som använder cache för att komma åt data. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Kombinerar ett annat Workbook-objekt. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Kopierar data från ett käll-Workbook-objekt. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Kopierar ett annat Workbook-objekt. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Kopierar temat från en annan Workbook. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Skapar inbyggd stil enligt given typ. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Skapar ett [`CellsColor`](../cellscolor/) objekt. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Skapar en ny stil. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Skapar en ny stil. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Anpassar temat. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | Exportera XML-data. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Exportera XML-data länkad av den specificerade XML-kartan. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Hämtar digital signatur från fil. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Hämtar alla teckensnitt i stilpoolen. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Hitta bäst matchande färg i aktuell palett. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Hämtar den namngivna stilen i stilpoolen. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Hämtar stilen i stilpoolen. Alla stilar i arbetsboken kommer att samlas i en pool. Det finns bara ett enkelt referensindex i cellerna. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Hämtar temafärg. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) Anger om denna arbetsbok innehåller externa länkar till andra datakällor. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Importerar/Uppdaterar en XML‑datafil i arbetsboken. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Importerar/Uppdaterar en XML‑datafil i arbetsboken. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Kontrollerar om en färg finns i paletten för kalkylbladet. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Slår samman namngivna format från den andra Excel-filen. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Analyserar alla formler som inte har analyserats när de laddades från mallfilen eller sattes i en cell. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Skyddar en arbetsbok. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Skyddar en delad arbetsbok. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | Uppdaterar länkade former, alla pivottabeller och diagram med pivottabellskälla. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data) Andra formler i arbetsboken kommer inte att beräknas rekursivt även om de användes av dynamiska matrisformler. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Uppdaterar dynamiska matrisformler(sprider sig till ett nytt område av intilliggande celler enligt aktuell data) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Tar bort digital signatur från detta kalkylblad. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolete.**) Tar bort alla externa länkar i arbetsboken. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Tar bort VBA/makro från detta kalkylblad. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Tar bort personlig information. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Ta bort alla oanvända format. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Ersätter cellers värden med ny data. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Ersätter cellers värden med ny data. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Ersätter cellers värden med data från en DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Ersätter en cells värde med ett nytt double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Ersätter en cells värde med ett nytt integer. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Ersätter en cells värde med en ny string. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Ersätter cellers värden med en double‑array. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Ersätter cellers värden med en integer‑array. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Ersätter en cells värde med en ny string. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Ersätter en cells värde med en ny string‑array. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Spara arbetsboken till disken. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Sparar arbetsboken till strömmen. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Sparar arbetsboken till strömmen. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Sparar arbetsboken till disken. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Sparar arbetsboken till disken. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Skapar resultatspridarket och överför det till klienten för att sedan öppna det i webbläsaren eller MS Workbook. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Skapar resultatspridarket och överför det till klienten för att sedan öppna det i webbläsaren eller MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Sparar Excel-filen till ett MemoryStream-objekt som en Excel97-2003 xls-fil och returnerar den. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Ställer in digital signatur för ett kalkylarksfil (Excel2007 och senare). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Ställ in krypteringsalternativ. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Ställer in temafärgen |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Startar sessionen som använder cache för att komma åt data. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Avskyddar en arbetsbok. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Avskyddar en delad arbetsbok. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Uppdaterar definitionen av anpassade funktioner. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | Om den här arbetsboken innehåller externa länkar till andra datakällor, kommer Aspose.Cells att försöka hämta den senaste datan från angivna källor. |

### Anmärkningar

Klassen Workbook betecknar ett Excel-kalkylblad. Varje kalkylblad kan innehålla flera arbetsblad. Grundfunktionen för klassen är att öppna och spara inhemska Excel-filer. Klassen har några avancerade funktioner som att kopiera data från andra arbetsböcker, kombinera två arbetsböcker, konvertera Excel till PDF, rendera Excel till bild och skydda Excel-kalkylbladet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // Skapa en ny Workbook-instans
            Workbook workbook = new Workbook();

            // Åtkomst till standardarbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in några egenskaper för arbetsboken
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Lägg till ett nytt arbetsblad
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Lägg till data i det nya arbetsbladet
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Ställ in några dokumentegenskaper
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Spara arbetsboken till en fil
            workbook.Save("WorkbookExample.xlsx");

            // Visa några egenskaper
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Kontrollera om arbetsboken är licensierad
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Kontrollera om arbetsboken är digitalt signerad
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Kontrollera om arbetsboken innehåller makron
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Kontrollera om arbetsboken har några spårade ändringar
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Kontrollera antalet stilar i stilpoolen
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Kontrollera temats namn
            Console.WriteLine("Theme: " + workbook.Theme);

            // Kontrollera om arbetsboken är skyddad med ett lösenord
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Kontrollera om arbetsboken innehåller externa länkar
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // Frigör arbetsboken
            workbook.Dispose();
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


