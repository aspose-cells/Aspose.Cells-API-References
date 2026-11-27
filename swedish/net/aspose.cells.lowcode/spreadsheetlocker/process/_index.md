---
title: "SpreadsheetLocker.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpreadsheetLocker‑metod. Låser kalkylbladsfil med angivna inställningar"
type: docs
url: /sv/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Låser kalkylbladsfilen med angivna inställningar.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | String | Mallfilen som ska låsas |
| resultFile | String | Den resulterande filen |
| openPassword | String | Lösenord för filkryptering |
| writePassword | String | Lösenord för skydd vid ändring av kalkylblad |

### Exempel

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
            // Förbered sökväg för resultatfil
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Utför Process‑metoden med strängparametrar direkt via typen
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
                // Rensa temporär mall
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Se även

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Låser kalkylbladsfilen med angivna inställningar.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för utdata och sparning. |
| openPassword | String | Lösenord för filkryptering |
| writePassword | String | Lösenord för skydd vid ändring av kalkylblad |

### Exempel

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
            
            // Bearbeta kalkylbladet med lås/upplåsningslösenord
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

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Låser kalkylbladsfilen med angivna inställningar.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för utdata och sparning. |
| openPassword | String | Lösenord för filkryptering |
| writePassword | String | Lösenord för skydd vid ändring av kalkylblad |
| workbookPassword | String | Lösenord för skydd av arbetsboken |
| workbookType | ProtectionType | Skyddstyp för att skydda arbetsboken |

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Låser kalkylbladsfilen med angivna inställningar.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för utdata och sparning. |
| leverantör | AbstractLowCodeProtectionProvider | Implementering för att tillhandahålla skyddsinställningar |

### Exempel

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
           
            // Förbered LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // Förbered LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Skapa en anpassad skyddsleverantör
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Anropa den statiska Process-metoden med angivna parametrar
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

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


