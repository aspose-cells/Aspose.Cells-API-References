---
title: "SpreadsheetConverter.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SpreadsheetConverter. Convierte el archivo de plantilla dado entre formatos de archivo de hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

Convierte el archivo de plantilla dado entre formatos de archivo de hoja de cálculo.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | String | El archivo de plantilla a convertir |
| resultFile | String | El archivo resultante |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            SpreadsheetConverter.Process("file1.xlsx", "SpreadsheetConverterMethodProcessWithStringStringDemo.xlsb");
        }
    }
}
```

### Ver también

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convierte entre diferentes formatos de archivo de hoja de cálculo.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones de salida y guardado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Crear opciones de carga con el archivo de entrada
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "file1.xlsx";

            // Crear opciones de guardado con el archivo de salida
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";

            // Ejecutar conversión
            SpreadsheetConverter.Process(loadOptions, saveOptions);
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


