---
title: "JsonUtility.ExportRangeToJson"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método JsonUtility. Exportando el rango a un archivo json"
type: docs
url: /es/net/aspose.cells.utility/jsonutility/exportrangetojson/
---
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}

Exportando el rango a un archivo json.

```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | El rango. |
| opciones | ExportRangeToJsonOptions | Las opciones de exportación. |

### Valor de retorno

El valor de la cadena json.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método ExportRangeToJson(Range range, JsonSaveOptions options). Esta propiedad será eliminada 6 meses después desde noviembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear un rango que cubra los datos
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Crea opciones de exportación
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.ExportAsString = true;

            // Exporta rango a JSON
            string json = JsonUtility.ExportRangeToJson(range, options);
            
            Console.WriteLine(json);
        }
    }
}
```

### Ver también

* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}

Exportando el rango a un archivo json.

```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | El rango. |
| opciones | JsonSaveOptions | Las opciones de exportación. |

### Valor de retorno

El valor de la cadena json.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeJsonSaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("New York");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["C3"].PutValue("London");

            // Crear rango (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 3);
            
            // Configurar opciones de exportación JSON
            JsonSaveOptions options = new JsonSaveOptions();
            options.ExportEmptyCells = true;
            options.HasHeaderRow = true;
            options.ExportNestedStructure = false;

            // Exporta rango a JSON
            string jsonOutput = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
            
            // Generar el resultado JSON
            Console.WriteLine(jsonOutput);
        }
    }
}
```

### Ver también

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


