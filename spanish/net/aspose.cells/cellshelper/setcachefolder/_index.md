---
title: "CellsHelper.SetCacheFolder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Establece la carpeta para archivos temporales que pueden usarse como caché de datos"
type: docs
url: /es/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Establece la carpeta para archivos temporales que pueden usarse como caché de datos.

```csharp
public static void SetCacheFolder(string cache)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| caché | String | Carpeta para archivos temporales que pueden usarse como caché de datos. |

### Observaciones

Los archivos de caché se utilizan generalmente para algunas funciones relacionadas con el rendimiento de la memoria, como guardar conjuntos de datos grandes en un archivo xls, o usar el modo de memoria con caché de archivos para el modelo de celdas.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodSetCacheFolderWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un directorio temporal para la caché
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // Establecer la carpeta de caché usando CellsHelper
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Verificar que la carpeta de caché se haya establecido
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // Crear un libro de trabajo simple para demostrar la funcionalidad
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Guarda el libro de trabajo
                workbook.Save("CacheFolderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with cache folder configured.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting cache folder: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


