---
title: "SpreadsheetLocker.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SpreadsheetLocker. Blocca il file del foglio di calcolo con le impostazioni specificate"
type: docs
url: /it/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Blocca il file del foglio di calcolo con le impostazioni specificate.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | String | Il file modello da bloccare |
| resultFile | String | Il file risultante |
| openPassword | String | Password per la crittografia del file |
| writePassword | String | Password per la protezione della modifica del foglio di calcolo |

### Esempi

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
            // Prepara il percorso del file di risultato
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Esegui il metodo Process con parametri stringa direttamente usando il tipo
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
                // Pulisci il modello temporaneo
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Vedi anche

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Blocca il file del foglio di calcolo con le impostazioni specificate.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |
| openPassword | String | Password per la crittografia del file |
| writePassword | String | Password per la protezione della modifica del foglio di calcolo |

### Esempi

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
            
            // Elabora il foglio di calcolo con password di blocco/sblocco
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

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Blocca il file del foglio di calcolo con le impostazioni specificate.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |
| openPassword | String | Password per la crittografia del file |
| writePassword | String | Password per la protezione della modifica del foglio di calcolo |
| workbookPassword | String | Password per la protezione della cartella di lavoro |
| workbookType | ProtectionType | Tipo di protezione per la cartella di lavoro |

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Blocca il file del foglio di calcolo con le impostazioni specificate.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |
| provider | AbstractLowCodeProtectionProvider | Implementazione per fornire le impostazioni di protezione |

### Esempi

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
           
            // Prepara LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // Prepara LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Crea un provider di protezione personalizzato
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Chiama il metodo statico Process con i parametri specificati
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

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


