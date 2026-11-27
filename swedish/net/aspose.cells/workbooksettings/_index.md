---
title: "Klassen WorkbookSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WorkbookSettings-klass. Representerar alla inställningar för arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Representerar alla inställningar för arbetsboken.

```csharp
public class WorkbookSettings : IDisposable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Hämtar och anger författaren till filen. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Anger ett booleskt värde som visar att programmet automatiskt komprimerar bilder i arbetsboken. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Anger om filen är markerad för automatisk återställning. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Anger den inkrementella offentliga releasen av programmet. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Anger om kompatibilitet med tidigare versioner ska kontrolleras när arbetsboken sparas. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Anger om anpassat talformat ska kontrolleras när Style.Custom sätts. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att en strängvärde längre än 32 K matas in. När du matar in ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Anger OOXML-versionen för utdokumentet. Standardvärdet är Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | Anger om programmet senast sparade arbetsboksfilen efter en krasch. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Hämtar eller anger systemets kulturinformation. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | Anger om programmet senast öppnade arbetsboken för dataräddning. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Hämtar eller anger ett värde som visar om arbetsboken använder 1904-datersystemet. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Hämtar och anger standardupplösning för bild. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Hämtar inställningarna för standardvärden för stilrelaterade egenskaper i denna arbetsbok. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Anger om redigeringsbilddata ska kastas. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Anger om och hur objekt ska visas i arbetsboken. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Aktivera makron; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | Hämtar eller anger den första synliga arbetsbladfliken. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Hämtar inställningarna för formelrelaterade funktioner. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Hämtar och anger globaliseringsinställningarna. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | Hämtar och anger om fältlistan för pivottabellen ska döljas. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Anger om arbetsboken ska krypteras med standardlösenord när struktur och fönster i arbetsboken är låsta. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Hämtar ett värde som visar om ett lösenord krävs för att öppna denna arbetsbok. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Anger om denna arbetsbok är dold. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Hämtar eller anger ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en horisontell rullningslist. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Anger om det genererade kalkylbladet kommer att öppnas minimerat. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Hämtar ett värde som indikerar om strukturen eller fönstret i arbetsboken är skyddat. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Hämtar eller anger ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en vertikal rullningslist. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Hämtar eller anger användargränssnittsspråket för arbetsbokens version baserat på landskoden som har sparat filen. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Hämtar det maximala kolumnindexet, nollbaserat. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Hämtar det maximala radindexet, nollbaserat. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Hämtar och anger det maximala radnumret för delad formel. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Hämtar och anger begränsningen av unika objekt per fält |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Hämtar eller anger minnesanvändningsalternativen. Det nya alternativet kommer att användas som standardalternativ för nysskapade arbetsblad men påverkar inte befintliga arbetsblad. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Hämtar eller anger decimalavgränsaren för formatering/parsning av numeriska värden. Standard är decimalavgränsaren för aktuell region. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Hämtar eller anger tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. Standard är gruppavgränsaren för aktuell region. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Hämtar och anger standardpappersstorleken för utskrift. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Anger arbetsbokens filkrypteringslösenord. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Indikerar om datapunkts egenskaper och datamärkningar i alla diagram i denna arbetsbok följer deras referens. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Hämtar skyddstypen för arbetsboken. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Indikerar om inställning av egenskapen [`QuotePrefix`](../style/quoteprefix/) när man anger strängvärdet (som börjar med ett enkelt citattecken) till cellen |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Hämtar eller anger de regionala inställningarna för arbetsboken. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | Sant om personlig information kan tas bort från den angivna arbetsboken. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Indikerar om programmet senast öppnade arbetsboken i säkert eller reparationsläge. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Hämtar och anger strömleverantören för extern resurs, såsom att ladda bilddata för bild av typen "LinkToFile". |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | Hämtar och anger hur programmet visar former i denna arbetsbok |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Hämtar eller anger ett värde som indikerar om arbetsboken är delad. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Bredd på arbetsbladets flikrad (i 1/1000 av fönsterbredden). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Hämtar eller anger ett värde om arbetsbokens flikar visas. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) Hämtar och anger antalet signifikanta siffror. Standardvärdet är [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Hämtar och anger typen av signifikanta siffror för att skriva ut numeriska värden i den här arbetsboken. Standardvärdet är [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Hämtar alternativen för smart-taggen. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) Hämtar och anger strömleverantören för extern resurs. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Anger om gränsen för intilliggande celler ska uppdateras. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Hämtar och anger hur externa länkar uppdateras när arbetsboken öppnas. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | Fönstrets höjd, i enheten punkt. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | Fönstrets höjd, i enheten centimeter. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | Fönstrets höjd, i enheten tum. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret, i enheten punkt. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten centimeter. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten tum. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | Avståndet från övre kanten av klientområdet till övre kanten av fönstret, i enheten punkt. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | Avståndet från övre kanten av klientområdet till övre kanten av fönstret, i enheten centimeter. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | Avståndet från övre kanten av klientområdet till övre kanten av fönstret, i enheten tum. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | Fönstrets bredd, i enheten punkt. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | Fönstrets bredd, i enheten centimeter. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | Fönstrets bredd, i enheten tum. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | Anger om den ska vara kompatibel med WPS. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Tillhandahåller åtkomst till arbetsbokens skrivskyddsalternativ. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Frigör resurser. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Hämtar standardtemats typsnittsnamn. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Ange typen av utskriftsorientering för hela arbetsboken. |

### Exempel

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Skapa en ny arbetsbok
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Lägg till lite exempeldata
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // Åtkomst till WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // Ange olika inställningar
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Spara arbetsboken
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


