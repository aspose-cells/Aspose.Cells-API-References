---
title: WorkbookSettings
second_title: Aspose.Cells för .NET API-referens
description: Representerar alla inställningar i arbetsboken.
type: docs
weight: 6500
url: /sv/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Representerar alla inställningar i arbetsboken.

```csharp
public class WorkbookSettings : IDisposable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Hämtar och ställer in författaren till filen. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Anger ett booleskt värde som anger att programmet automatiskt komprimerade bilder i arbetsboken. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Indikerar om filen är markerad för automatisk återställning. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Anger den inkrementella offentliga versionen av programmet. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Indikerar om du kontrollerar kompatibilitet med tidigare versioner när du sparar arbetsbok. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Indikerar om anpassat talformat kontrolleras vid inställning av Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Om kontrollera begränsningen av excel-fil när användaren ändrar cellrelaterade objekt. Till exempel tillåter excel inte inmatning av strängvärden som är längre än 32K. När du matar in ett värde längre än 32K såsom av Cell.PutValue(sträng), om detta egenskapen är sant får du ett undantag. Om den här egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan mata ut hela strängvärdet för andra filformat som CSV. Men om du har angett ett sådant värde som är ogiltigt för Excel-filformat, du bör inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå ett oväntat fel för den genererade excel-filen. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Anger OOXML-versionen för utdatadokumentet. Standardvärdet är Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | anger om programmet senast sparade arbetsboksfilen efter en krasch. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Hämtar eller ställer in systemkulturinformationen. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | anger om programmet senast öppnade arbetsboken för dataåterställning. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Hämtar eller ställer in ett värde som representerar om arbetsboken använder 1904-datumsystemet. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Indikerar om och hur objekt ska visas i arbetsboken. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Aktivera makron; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | Hämtar eller ställer in den första synliga kalkylbladsfliken. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Hämtar inställningarna för formelrelaterade funktioner. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Hämtar och ställer in globaliseringsinställningarna. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | Hämtar och ställer in om fältlistan för pivottabellen ska döljas. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Indikerar om kryptering av arbetsboken med standardlösenord om arbetsbokens struktur och Windows är låsta. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Får ett värde som indikerar om ett lösenord krävs för att öppna denna arbetsbok. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Indikerar om denna arbetsbok är dold. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Hämtar eller ställer in ett värde som anger om det genererade kalkylarket kommer att innehålla en horisontell rullningslist. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Representerar om det genererade kalkylarket kommer att öppnas Minimerat. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Får ett värde som indikerar om strukturen eller fönstret i arbetsboken är skyddad. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Hämtar eller ställer in ett värde som anger om det genererade kalkylarket kommer att innehålla en vertikal rullningslist. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Hämtar eller ställer in användargränssnittsspråket för versionen av arbetsboken baserat på CountryCode som har sparat filen. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Hämtar max kolumnindex, nollbaserat. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Hämtar max radindex, nollbaserat. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Hämtar och ställer in det maximala radnumret för delad formel. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Hämtar eller ställer in alternativen för minnesanvändning. Det nya alternativet kommer att användas som standardalternativ för nyskapade kalkylblad men träder inte i kraft för befintliga kalkylblad. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Hämtar eller ställer in decimalavgränsaren för formatering/analys av numeriska värden. Standard är decimalavgränsaren för aktuell region. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Hämtar eller ställer in tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. Standard är gruppseparatorn för aktuell region. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Hämtar och ställer in standardstorleken för utskriftspapper. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Representerar arbetsboksfilkrypteringslösenord. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Hämtar skyddstypen för arbetsboken. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Indikerar om inställning[`QuotePrefix`](../style/quoteprefix) egenskap när du anger strängvärdet (som börjar med enkla citattecken) till cellen |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Hämtar eller ställer in de regionala inställningarna för arbetsboken. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | Sant om personlig information kan tas bort från den angivna arbetsboken. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Indikerar om programmet senast öppnade arbetsboken i säkert läge eller reparationsläge. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | Hämtar och ställer in strömleverantören för extern resurs, som att ladda bilddata för bild av typen "LinkToFile". |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Hämtar eller ställer in ett värde som anger om arbetsboken är delad. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Bredden på kalkylbladets flikfält (i 1/1000 av fönstrets bredd). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Hämta eller ställer in ett värde oavsett om arbetsboksflikarna visas. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Hämtar och ställer in antalet signifikanta siffror. Standardvärdet är[`SignificantDigits`](../cellshelper/significantdigits) . |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Indikerar om uppdatering av angränsande cellers kantlinje. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Hämtar och ställer in hur externa länkar uppdateras när arbetsboken öppnas. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Får eller ställer in varningsåteruppringning. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | Höjden på fönstret, i punktenhet. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | Höjden på fönstret, i centimeterenhet. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | Höjden på fönstret, i enhet tum. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | Avståndet från den vänstra kanten av klientområdet till den vänstra kanten av fönstret, i punktenhet. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | Avståndet från klientområdets vänstra kant till fönstrets vänstra kant. I centimeterenhet. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | Avståndet från den vänstra kanten av klientområdet till den vänstra kanten av fönstret. I enhet av tum. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | Avståndet från klientområdets övre kant till fönstrets övre kant, i punktenhet. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | Avståndet från klientområdets övre kant till fönstrets övre kant, i centimeterenhet. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | Avståndet från klientområdets övre kant till fönstrets övre kant, i tumenhet. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | Bredden på fönstret, i punktenhet. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | Fönstrets bredd, i centimeterenhet. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | Bredden på fönstret, i enhet tum. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Ger åtkomst till arbetsbokens skrivskyddsalternativ. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Frigör resurser. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Får standardtemans teckensnittsnamn. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Ställ in typen av utskriftsorientering för hela arbetsboken. |

### Exempel

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

//gör dina affärer

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'göra dina affärer
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
