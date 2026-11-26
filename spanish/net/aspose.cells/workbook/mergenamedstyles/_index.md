---
title: "Workbook.MergeNamedStyles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Fusiona estilos con nombre del otro archivo Excel"
type: docs
url: /es/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Fusiona estilos nombrados del otro archivo Excel.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Libro de trabajo | El otro archivo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Crear el libro de trabajo de destino (el que recibirá los estilos con nombre)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Agregar algunos datos al libro de trabajo de destino para contexto
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Crear el libro de trabajo fuente (el que contiene los estilos con nombre para fusionar)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Agregar algunos datos al libro de trabajo fuente para contexto
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // Fusionar estilos con nombre de sourceWorkbook en targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Guardar el libro de trabajo resultante
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


