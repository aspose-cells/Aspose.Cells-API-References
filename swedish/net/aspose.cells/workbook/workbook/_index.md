---
title: "Workbook.Workbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook‑konstruktor. Initierar en ny instans av klassen Workbook"
type: docs
url: /sv/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Initierar en ny instans av klassen [`Workbook`](../).

```csharp
public Workbook()
```

### Anmärkningar

Standardfilformatet är Xlsx. Om du vill skapa andra filtyper, använd Workbook(FileFormatType).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med hjälp av konstruktorn
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Spara arbetsboken
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Initierar en ny instans av klassen [`Workbook`](../).

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileFormatType | FileFormatType | Det nya filformatet. |

### Anmärkningar

Standardfilformatet är Excel97To2003.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med XLSX‑filformat
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sätt in lite data i cell A1
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

Initierar en ny tom instans av klassen [`Workbook`](../) med alternativ

```csharp
public Workbook(LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LoadOptions | Alternativen. |

### Se även

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

Initierar en ny instans av klassen [`Workbook`](../) och öppnar en fil.

```csharp
public Workbook(string file)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | String | Filnamnet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Sökvägen till dokumentkatalogen.
            string dataDir = "Your Document Directory";

            // Skapa en Workbook från en befintlig Excel‑fil
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa viss kalkylbladsinformation
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // Spara arbetsboken i MHTML-format
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // Skapa en annan arbetsbok från den sparade MHTML-filen
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

Initierar en ny instans av klassen [`Workbook`](../) och öppnar en ström.

```csharp
public Workbook(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Strömmen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // Skapa en exempel‑Excel‑fil i minnet
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // Skapa en ny Workbook‑instans med Stream‑konstruktorn
                Workbook workbook = new Workbook(sampleStream);

                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];

                // Visa den inlästa datan
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // Spara arbetsboken till en fil
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

Initierar en ny instans av klassen [`Workbook`](../) och öppnar en fil.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | String | Filnamnet. |
| loadOptions | LoadOptions | Laddningsalternativen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ utan LightCellsDataHandler
            LoadOptions loadOptions = new LoadOptions();

            // Initiera arbetsboken med filsökväg och laddningsalternativ
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Visa att arbetsboken är laddad genom att läsa antalet kalkylblad
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### Se även

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

Initierar en ny instans av klassen [`Workbook`](../) och öppnar en ström.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Strömmen. |
| loadOptions | LoadOptions | Laddningsalternativen |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en exempel‑Excel‑fil i minnet
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // Skapa LoadOptions med specifika inställningar
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // Skapa en Workbook‑instans med #ctor och Stream samt LoadOptions
                Workbook workbook = new Workbook(stream, loadOptions);

                // Visa grundläggande information om den laddade arbetsboken
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // Visa viss cellinnehåll om det finns tillgängligt
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // Skapa en enkel Excel‑fil i minnet för demonstration
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### Se även

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


