---
title: SpreadsheetLocker.Process
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetLocker method. Locks spreadsheet file with specified settings
type: docs
url: /net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be locked |
| resultFile | String | The resultant file |
| openPassword | String | Password for file encryption |
| writePassword | String | Password for protection of modifying spreadsheet |

### Examples

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
            // Prepare result file path
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Execute Process method with string parameters directly using the type
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
                // Clean up temporary template
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### See Also

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
| openPassword | String | Password for file encryption |
| writePassword | String | Password for protection of modifying spreadsheet |

### Examples

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
            
            // Process the spreadsheet with lock/unlock passwords
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

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
| openPassword | String | Password for file encryption |
| writePassword | String | Password for protection of modifying spreadsheet |
| workbookPassword | String | Password for protection of the workbook |
| workbookType | ProtectionType | Protection type to protect the workbook |

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Locks spreadsheet file with specified settings.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
| provider | AbstractLowCodeProtectionProvider | Implementation to provide protections settings |

### Examples

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
           
            // Prepare LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // Prepare LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Create a custom protection provider
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Call the static Process method with specified parameters
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

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


