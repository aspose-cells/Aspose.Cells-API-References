---
title: "SpreadsheetMerger.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SpreadsheetMerger. Fusionar los archivos de plantilla proporcionados"
type: docs
url: /es/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

Combinar los archivos de plantilla proporcionados.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFiles | String[] | Los archivos de plantilla a fusionar |
| resultFile | String | El archivo resultante |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithStringArrayStringDemo
    {
        public static void Run()
        {
            // Crear archivos de plantilla de ejemplo
            CreateTemplateFile("template1.xlsx", "Data from Template 1");
            CreateTemplateFile("template2.xlsx", "Data from Template 2");

            string[] templateFiles = { "template1.xlsx", "template2.xlsx" };
            string resultFile = "merged_output.xlsx";

            try
            {
                SpreadsheetMerger.Process(templateFiles, resultFile);

                Console.WriteLine($"Process method merged {templateFiles.Length} files into {resultFile}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Ver también

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

Fusiona varios archivos de plantilla en uno.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | LowCodeMergeOptions | Opciones para fusionar archivos |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithLowCodeMergeOptDemo
    {
        public static void Run()
        {
            // Preparar dos archivos de plantilla simples que serán fusionados.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // Crear una instancia de la clase de opciones.
                // La clase LowCodeMergeOptions es parte de Aspose.Cells.LowCode.
                // Para esta demostración usamos el constructor predeterminado.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // Llame al método Process que acepta LowCodeMergeOptions.
                SpreadsheetMerger.Process(options);

                Console.WriteLine("Process method invoked successfully with LowCodeMergeOptions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Ver también

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


