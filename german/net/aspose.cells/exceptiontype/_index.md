---
title: "Aufzählung ExceptionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExceptionType-Enum. Stellt einen benutzerdefinierten Ausnahme-Typcode dar"
type: docs
url: /de/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Stellt den Code des benutzerdefinierten Ausnahmetyps dar.

```csharp
public enum ExceptionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Chart | `0` | Ungültige Diagrammeinstellung. |
| DataType | `1` | Ungültige Datentyp-Einstellung. |
| DataValidation | `2` | Ungültige Datenvalidierungseinstellung. |
| ConditionalFormatting | `3` | Ungültige Datenvalidierungseinstellung. |
| FileFormat | `4` | Ungültiges Dateiformat. |
| Formula | `5` | Ungültige Formel. |
| InvalidData | `6` | Ungültige Daten. |
| InvalidOperator | `7` | Ungültiger Operator. |
| IncorrectPassword | `8` | Falsches Passwort. |
| License | `9` | Lizenzbezogene Fehler. |
| Limitation | `10` | Fehler wegen Überschreitung der MS-Excel-Beschränkung. |
| PageSetup | `11` | Ungültige Seiteneinrichtung. |
| PivotTable | `12` | Ungültige PivotTable-Einstellung. |
| Shape | `13` | Ungültige Einstellung des Zeichenobjekts. |
| Sparkline | `14` | Ungültige Sparkline-Objekteinstellung. |
| SheetName | `15` | Ungültiger Arbeitsblattname. |
| SheetType | `16` | Ungültiger Arbeitsblatttyp. |
| Interrupted | `17` | Der Vorgang wurde unterbrochen. |
| IO | `18` | Die Datei ist ungültig. |
| Permission | `19` | Berechtigung ist erforderlich, um diese Datei zu öffnen. |
| UnsupportedFeature | `20` | Nicht unterstützte Funktion. |
| UnsupportedStream | `21` | Nicht unterstützter Stream zum Öffnen. |
| UndisclosedInformation | `22` | Dateien enthalten einige nicht offengelegte Informationen. |
| FileCorrupted | `23` | Dateiinhalt ist beschädigt. |
| DefinedName | `25` | Ungültiger definierter Name |
| Font | `26` | Ungültige Schriftart |
| AutoFilter | `27` | Ungültige Auto-Filter-Einstellung. |
| FontSubstitution | `28` | Schriftart-Substitutions-Warnungstyp, wenn eine Schriftart nicht gefunden wurde, dieser Warnungstyp kann abgerufen werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExceptionTypeDemo
    {
        public static void ExceptionTypeExample()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();

                // Versuch, einen ungültigen Arbeitsblattnamen zu setzen, um eine Ausnahme auszulösen
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Speichere die Arbeitsmappe
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // Behandle die CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // Überprüfe den Typ der Ausnahme
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Füge bei Bedarf weitere Fälle für verschiedene Ausnahmetypen hinzu
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Behandle alle anderen Ausnahmen
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


