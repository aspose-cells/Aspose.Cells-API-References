---
title: "Workbook.FileFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene y establece el formato de archivo"
type: docs
url: /es/net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Obtiene y establece el formato del archivo.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileFormatDemo
    {
        public static void Run()
        {
            // Crear un archivo CSV de ejemplo
            string csvFile = "sample.csv";
            File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");

            // Crear un archivo XLSX de ejemplo
            string xlsxFile = "sample.xlsx";
            using (Workbook wb = new Workbook())
            {
                wb.Worksheets[0].Cells["A1"].PutValue("Test");
                wb.Save(xlsxFile);
            }

            // Demostrar la propiedad FileFormat
            ProcessWorkbook(csvFile);
            ProcessWorkbook(xlsxFile);

            // Limpieza
            File.Delete(csvFile);
            File.Delete(xlsxFile);
        }

        private static void ProcessWorkbook(string filePath)
        {
            using (Workbook wb = new Workbook(filePath))
            {
                Console.WriteLine($"Processing file: {filePath}");
                Console.WriteLine($"File format: {wb.FileFormat}");

                if (wb.FileFormat == FileFormatType.Csv)
                {
                    Console.WriteLine("This is a CSV file");
                    // Procesamiento adicional específico de CSV
                }
                else if (wb.FileFormat == FileFormatType.Xlsx)
                {
                    Console.WriteLine("This is an XLSX file");
                    // Procesamiento adicional específico de XLSX
                }
            }
        }
    }
}
```

### Ver también

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


