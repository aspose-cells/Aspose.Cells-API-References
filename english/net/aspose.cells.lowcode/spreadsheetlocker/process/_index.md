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
namespace AsposeCellsExamples.SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
    {
        public static void Run()
        {
            // Create and save a template workbook
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].Value = "Confidential Data";
            string templatePath = "template.xlsx";
            templateWorkbook.Save(templatePath);

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
// Called: SpreadsheetLocker.Process(new LowCodeLoadOptions() { InputStream = stream },
private void SpreadsheetLocker_Method_Process(Stream stream, string fnTail)
        {
            SpreadsheetLocker.Process(new LowCodeLoadOptions() { InputStream = stream },
                new LowCodeSaveOptions()
                {
                    OutputFile = Constants.checkPath + "License/LowCodeLock" + fnTail,
                }, "123456", "234567");
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

### Examples

```csharp
namespace AsposeCellsExamples.SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Create LowCodeLoadOptions and LowCodeSaveOptions instances
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();

            // Define protection parameters
            string openPassword = "userOpen123";
            string writePassword = "userWrite123";
            string workbookPassword = "workbookProtect123";
            ProtectionType protectionType = ProtectionType.All;

            try
            {
                // Call the Process method directly without instantiating SpreadsheetLocker
                SpreadsheetLocker.Process(loadOptions, saveOptions, openPassword, writePassword, workbookPassword, protectionType);
                
                Console.WriteLine("Spreadsheet processed successfully with document protection settings.");
            }
            catch (CellsException ex)
            {
                Console.WriteLine($"Aspose.Cells error during processing: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"General error: {ex.Message}");
            }
        }
    }
}
```

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
namespace AsposeCellsExamples.SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Prepare LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();

            // Prepare LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;

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

            // Save the result
            workbook.Save("ProcessWithLowCodeOptionsDemo.xlsx");
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


