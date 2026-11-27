---
title: "JsonUtility.ExportRangeToJson"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonUtility-metod. Exporterar området till en json-fil"
type: docs
url: /sv/net/aspose.cells.utility/jsonutility/exportrangetojson/
---
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}

Exporterar området till json-fil.

```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Området. |
| alternativ | ExportRangeToJsonOptions | Exportalternativen. |

### Returvärde

json-strängvärdet.

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället ExportRangeToJson(Range range, JsonSaveOptions options)-metoden. Denna egenskap kommer att tas bort 6 månader senare sedan november 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa ett område som täcker data
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Skapa exportalternativ
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.ExportAsString = true;

            // Exportera område till JSON
            string json = JsonUtility.ExportRangeToJson(range, options);
            
            Console.WriteLine(json);
        }
    }
}
```

### Se även

* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}

Exporterar området till json-fil.

```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Området. |
| alternativ | JsonSaveOptions | Exportalternativen. |

### Returvärde

json-strängvärdet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeJsonSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("New York");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["C3"].PutValue("London");

            // Skapa område (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 3);
            
            // Konfigurera JSON-exportalternativ
            JsonSaveOptions options = new JsonSaveOptions();
            options.ExportEmptyCells = true;
            options.HasHeaderRow = true;
            options.ExportNestedStructure = false;

            // Exportera område till JSON
            string jsonOutput = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
            
            // Skriv ut JSON-resultatet
            Console.WriteLine(jsonOutput);
        }
    }
}
```

### Se även

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


