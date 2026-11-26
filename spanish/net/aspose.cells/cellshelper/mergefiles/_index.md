---
title: "CellsHelper.MergeFiles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Fusiona algunos archivos xls grandes en un archivo xls"
type: docs
url: /es/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

Fusiona varios archivos xls grandes en un archivo xls.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| archivos | String[] | Los archivos. |
| cachedFile | String | El archivo en caché. |
| destFile | String | El archivo de destino. |

### Observaciones

Este método solo admite fusionar datos, estilos y fórmulas en el nuevo archivo. El archivo en caché se utiliza para almacenar algunos datos temporales.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodMergeFilesWithStringStringDemo
    {
        public static void Run()
        {
            // Crear archivos Excel temporales para fusionar
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // Crear libros de trabajo de muestra
            Workbook workbook1 = new Workbook();
            workbook1.Worksheets[0].Cells["A1"].PutValue("File 1 Content");
            workbook1.Save(filesToMerge[0]);

            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("File 2 Content");
            workbook2.Save(filesToMerge[1]);

            string cachedFile = "CacheFile.tmp";
            string outputFile = "MergedOutput.xlsx";

            try
            {
                // Llamar a MergeFiles con los parámetros String[], String, String
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // Verificar el archivo fusionado
                Workbook mergedWorkbook = new Workbook(outputFile);
                Console.WriteLine("Merged content:");
                Console.WriteLine(mergedWorkbook.Worksheets[0].Cells["A1"].StringValue);
                Console.WriteLine(mergedWorkbook.Worksheets[1].Cells["A1"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error merging files: {ex.Message}");
            }
            finally
            {
                // Limpia los archivos temporales
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


