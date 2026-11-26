---
title: "CellsHelper.GetCacheFolder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene la carpeta para archivos temporales que pueden usarse como caché de datos"
type: docs
url: /es/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Obtiene la carpeta para archivos temporales que pueden usarse como caché de datos.

```csharp
public static string GetCacheFolder()
```

### Valor de retorno

Carpeta para los archivos de caché que se ha especificado. Si no se ha especificado, se devolverá null y se utilizará la ruta temporal del sistema cuando sea necesario.

### Observaciones

Los archivos de caché se utilizan generalmente para algunas funciones relacionadas con el rendimiento de la memoria, como guardar conjuntos de datos grandes en un archivo xls, o usar el modo de memoria con caché de archivos para el modelo de celdas.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetCacheFolderDemo
    {
        public static void Run()
        {
            try
            {
                // Obtener la ruta actual de la carpeta de caché
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Mostrar la ruta de la carpeta de caché
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // Opcionalmente establecer una nueva carpeta de caché (demostrando el método relacionado)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Verificar el cambio
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Revertir al original (opcional)
                CellsHelper.SetCacheFolder(cacheFolder);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with cache folder: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


