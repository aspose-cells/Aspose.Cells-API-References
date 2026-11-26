---
title: "IFilePathProvider.GetFullName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IFilePathProvider. Obtiene la ruta completa del archivo por nombre de Worksheet al exportar Worksheet a HTML por separado. Así, las referencias entre las Worksheets pueden exportarse correctamente"
type: docs
url: /es/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

Obtiene la ruta completa del archivo por nombre de hoja de cálculo al exportar la hoja de cálculo a HTML por separado. Así, las referencias entre las hojas de cálculo pueden exportarse correctamente.

```csharp
public string GetFullName(string sheetName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | String | Nombre de la hoja de cálculo |

### Valor de retorno

la ruta completa del archivo

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // Crear una implementación personalizada de IFilePathProvider
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // Llamar al método GetFullName con el nombre de una hoja
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // Mostrar el resultado
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Implementación simple que devuelve una ruta combinando el nombre de la hoja con un directorio
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### Ver también

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


