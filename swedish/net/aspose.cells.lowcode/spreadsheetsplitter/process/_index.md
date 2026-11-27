---
title: "SpreadsheetSplitter.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpreadsheetSplitter‑metod. Delar upp given mallfil i flera delar"
type: docs
url: /sv/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Delar upp given mallfil i flera delar.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | String | Mallfilen som ska delas |
| resultFile | String | Den resulterande filen (namnmönster) |

### Anmärkningar

Utdatafilerna kommer att byggas från den angivna resulterande filen genom att lägga till sekvensnummer för bladet och den delade delen. Till exempel, om den angivna utdatafilen är Split.xlsx, kommer de genererade filerna att vara Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med flera kalkylblad
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // Spara som mallfil
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // Definiera resultatutmatningsmönster
            string resultPattern = "SplitResult_";
            
            try
            {
                // Processa mallen direkt med den statiska metoden
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Delar upp kalkylbladsfil i flera delar.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | LowCodeSplitOptions | Alternativ för att dela kalkylblad |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // Initiera delningsalternativ
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // Utför kalkylbladsuppdelning med statisk metod
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
        }
    }

    // Konkret implementation av AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implementera den erforderliga abstrakta metoden
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Se även

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


