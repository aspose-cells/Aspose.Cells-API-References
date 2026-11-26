---
title: "LoadOptions.LoadFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene el formato de carga"
type: docs
url: /es/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

Obtiene el formato de carga.

```csharp
public LoadFormat LoadFormat { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Crea un archivo CSV de ejemplo
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // Crear LoadOptions para el formato CSV y mostrar la propiedad
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // Cargar CSV con opciones correctas
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // Crear LoadOptions para el formato XLSX y mostrar la propiedad
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // Crear/guardar archivo XLSX de ejemplo
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // Cargar XLSX con opciones correctas
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // Limpiar archivos temporales
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


