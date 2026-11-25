---
title: "JsonUtility.ExportRangeToJson"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo JsonUtility. Esportazione dell'intervallo in un file json"
type: docs
url: /it/net/aspose.cells.utility/jsonutility/exportrangetojson/
---
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}

Esportazione dell'intervallo in un file json.

```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo. |
| opzioni | ExportRangeToJsonOptions | Le opzioni di esportazione. |

### Valore di ritorno

Il valore della stringa json.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo ExportRangeToJson(Range range, JsonSaveOptions options). Questa proprietà sarà rimossa tra 6 mesi a partire da novembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un intervallo che copre i dati
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Crea opzioni di esportazione
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.ExportAsString = true;

            // Esporta intervallo in JSON
            string json = JsonUtility.ExportRangeToJson(range, options);
            
            Console.WriteLine(json);
        }
    }
}
```

### Vedi anche

* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}

Esportazione dell'intervallo in un file json.

```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo. |
| opzioni | JsonSaveOptions | Le opzioni di esportazione. |

### Valore di ritorno

Il valore della stringa json.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeJsonSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("New York");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["C3"].PutValue("London");

            // Crea intervallo (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 3);
            
            // Configura le opzioni di esportazione JSON
            JsonSaveOptions options = new JsonSaveOptions();
            options.ExportEmptyCells = true;
            options.HasHeaderRow = true;
            options.ExportNestedStructure = false;

            // Esporta intervallo in JSON
            string jsonOutput = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
            
            // Genera il risultato JSON
            Console.WriteLine(jsonOutput);
        }
    }
}
```

### Vedi anche

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


