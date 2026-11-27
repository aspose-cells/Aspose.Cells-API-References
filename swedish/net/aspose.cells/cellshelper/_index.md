---
title: "Klassen CellsHelper"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellsHelper-klass. Tillhandahåller hjälpfunktioner"
type: docs
url: /sv/net/aspose.cells/cellshelper/
---
## CellsHelper class

Tillhandahåller hjälpfunktioner.

```csharp
public class CellsHelper
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Hämtar eller anger den alternativa startvägen, som refereras till av vissa externa formelreferenser. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Hämtar eller anger fabriken för att skapa instanser med speciell implementation. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Hämtar DPI för maskinen. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Ställ in denna egenskap till True när du kör på en molnplattform, såsom: Azure, AWSLambda, etc. |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Hämtar eller anger bibliotekssökvägen som refereras till av vissa externa formelreferenser. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Hämtar och anger antalet signifikanta siffror. Standardvärdet är 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Hämtar och anger standardtypen av signifikanta siffror för utskrift av numeriska värden. Standardvärdet är G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Hämtar eller anger startvägen, som refereras till av vissa externa formelreferenser. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Lägg till tilläggsfunktion. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Hämtar cellnamn enligt dess rad- och kolumnindex. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Hämtar cellens rad- och kolumnindex enligt dess namn. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Hämtar kolumnnamn enligt kolumnindex. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Hämtar kolumnindex enligt kolumnnamn. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsolete.**) Konverterar A1-formeln för cellen till r1c1-formeln. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsolete.**) Konverterar r1c1-formeln för cellen till A1-formeln. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn returneras det. Annars kommer strängen att trunkeras om längden överskrider gränsen och ogiltiga tecken ersätts med ' ', sedan returneras det återuppbyggda strängvärdet. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn returneras det. Annars kommer strängen att trunkeras om längden överskrider gränsen och ogiltiga tecken ersätts med det angivna tecknet, sedan returneras det återuppbyggda strängvärdet. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Hämtar mappen för temporära filer som kan användas som datacache. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Konvertera dubbelvärdet till datum‑tidsvärdet. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Konvertera datum‑tiden till dubbelvärde. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Hämta textens bredd i enheten punkter. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Hämtar alla använda färger i arbetsboken. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Hämta utgivningsversionen. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Slår samman några stora xls‑filer till en xls‑fil. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Anger om bladnamnet ska omges av enkla citattecken |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Hämtar radnamn enligt radindex. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Hämtar radindex enligt radnamn. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Ställer in mappen för temporära filer som kan användas som datacache. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // Ställer in egenskaper för CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // Förutsatt att CustomImplementationFactory redan är definierad och instansierad någon annanstans
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Demonstrerar användning av CellsHelper‑egenskaper
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Exempel på användning av CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


