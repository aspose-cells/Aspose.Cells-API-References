---
title: "SpreadsheetLocker.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpreadsheetLocker Methode. Sperrt die Tabellenkalkulationsdatei mit den angegebenen Einstellungen"
type: docs
url: /de/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Sperrt die Tabellendatei mit den angegebenen Einstellungen.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | String | Die Vorlagendatei, die gesperrt werden soll |
| resultFile | String | Die resultierende Datei |
| openPassword | String | Passwort für die Dateiverschlüsselung |
| writePassword | String | Passwort zum Schutz vor Änderungen an der Tabellenkalkulation |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
    {
        public static void Run()
        {           
            string templatePath = "template.xlsx";            
            // Bereite den Pfad der Ergebnisdatei vor
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Führe die Process-Methode mit Zeichenkettenparametern direkt unter Verwendung des Typs aus
                SpreadsheetLocker.Process(
                    templateFile: templatePath,
                    resultFile: resultPath,
                    openPassword: "Open@123",
                    writePassword: "Write@456"
                );

                Console.WriteLine($"Spreadsheet secured successfully. Saved to: {Path.GetFullPath(resultPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error securing spreadsheet: {ex.Message}");
            }
            finally
            {
                // Bereinige die temporäre Vorlage
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Siehe auch

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Sperrt die Tabellendatei mit den angegebenen Einstellungen.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen für Ausgabe und Speichern |
| openPassword | String | Passwort für die Dateiverschlüsselung |
| writePassword | String | Passwort zum Schutz vor Änderungen an der Tabellenkalkulation |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            
            // Verarbeite die Tabellenkalkulation mit Sperr-/Entsperrkennwörtern
            SpreadsheetLocker.Process(
                new LowCodeLoadOptions() { InputFile = "input.xlsx" },
                new LowCodeSaveOptions() 
                { 
                    OutputFile = "output_locked.xlsx" 
                }, 
                "123456", 
                "234567");
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Sperrt die Tabellendatei mit den angegebenen Einstellungen.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen für Ausgabe und Speichern |
| openPassword | String | Passwort für die Dateiverschlüsselung |
| writePassword | String | Passwort zum Schutz vor Änderungen an der Tabellenkalkulation |
| workbookPassword | String | Kennwort zum Schutz der Arbeitsmappe |
| workbookType | ProtectionType | Schutztyp zum Schutz der Arbeitsmappe |

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Sperrt die Tabellendatei mit den angegebenen Einstellungen.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen für Ausgabe und Speichern |
| provider | AbstractLowCodeProtectionProvider | Implementierung zur Bereitstellung von Schutzeinstellungen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
           
            // Bereite LowCodeLoadOptions vor
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // Bereite LowCodeSaveOptions vor
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Erstelle einen benutzerdefinierten Schutzanbieter
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Rufe die statische Process-Methode mit den angegebenen Parametern auf
                SpreadsheetLocker.Process(loadOptions, saveOptions, provider);

                Console.WriteLine("Spreadsheet processed and protected successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error processing spreadsheet: {ex.Message}");
            }

        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override string GetOpenPassword()
            {
                return "open123";
            }

            public override string GetWritePassword()
            {
                return "write123";
            }

            public override string GetWorkbookPassword()
            {
                return "workbook123";
            }

            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.All;
            }
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


