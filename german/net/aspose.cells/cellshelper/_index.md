---
title: "Klasse CellsHelper"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellsHelper-Klasse. Stellt Hilfsfunktionen bereit"
type: docs
url: /de/net/aspose.cells/cellshelper/
---
## CellsHelper class

Stellt Hilfsfunktionen bereit.

```csharp
public class CellsHelper
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Liest oder setzt den alternativen Startpfad, auf den von einigen externen Formelbezügen verwiesen wird. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Liest oder setzt die Fabrik zum Erzeugen von Instanzen mit spezieller Implementierung. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Liest die DPI des Geräts. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud-Plattform laufen, z. B.: Azure, AWSLambda, etc, |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Liest oder setzt den Bibliothekspfad, auf den von einigen externen Formelbezügen verwiesen wird. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Liest und setzt die Anzahl signifikanter Stellen. Der Standardwert ist 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Liest und setzt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte. Der Standardwert ist G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Liest oder setzt den Startpfad, auf den von einigen externen Formelbezügen verwiesen wird. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Add-In-Funktion hinzufügen. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Ermittelt den Zellnamen anhand seiner Zeilen- und Spaltenindizes. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Ermittelt die Zeilen- und Spaltenindizes der Zelle anhand ihres Namens. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Ermittelt den Spaltennamen anhand des Spaltenindex. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Ermittelt den Spaltenindex anhand des Spaltennamens. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsolete.**) Konvertiert die A1-Formel der Zelle in die r1c1-Formel. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsolete.**) Konvertiert die r1c1-Formel der Zelle in die A1-Formel. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen Namen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette gekürzt, falls die Länge das Limit überschreitet, und ungültige Zeichen werden durch ein Leerzeichen (' ') ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen Namen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette gekürzt, falls die Länge das Limit überschreitet, und ungültige Zeichen werden durch das angegebene Zeichen ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Ermittelt den Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Konvertiert den Double-Wert in einen DateTime-Wert. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Konvertiert den DateTime-Wert in einen Double-Wert. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Ermittelt die Breite des Textes in Punkt. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Ermittelt alle im Arbeitsbuch verwendeten Farben. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Ermittelt die Release-Version. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Führt mehrere große XLS-Dateien zu einer XLS-Datei zusammen. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Gibt an, ob der Blattname in einfache Anführungszeichen eingeschlossen werden soll. |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Ermittelt den Zeilennamen anhand des Zeilenindex. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Ermittelt den Zeilenindex anhand des Zeilennamens. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Setzt den Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // Einstellen von Eigenschaften von CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // Angenommen, CustomImplementationFactory ist bereits an anderer Stelle definiert und instanziiert.
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Demonstration der Verwendung von CellsHelper-Eigenschaften
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Beispiel für die Verwendung von CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


