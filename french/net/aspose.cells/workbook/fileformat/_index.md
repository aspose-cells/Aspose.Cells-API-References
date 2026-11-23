---
title: "Workbook.FileFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient et définit le format de fichier"
type: docs
url: /fr/net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Obtient et définit le format de fichier.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Exemples

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
            // Créer un fichier CSV d'exemple
            string csvFile = "sample.csv";
            File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");

            // Créer un fichier XLSX d'exemple
            string xlsxFile = "sample.xlsx";
            using (Workbook wb = new Workbook())
            {
                wb.Worksheets[0].Cells["A1"].PutValue("Test");
                wb.Save(xlsxFile);
            }

            // Démontrer la propriété FileFormat
            ProcessWorkbook(csvFile);
            ProcessWorkbook(xlsxFile);

            // Nettoyage
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
                    // Traitement supplémentaire spécifique au CSV
                }
                else if (wb.FileFormat == FileFormatType.Xlsx)
                {
                    Console.WriteLine("This is an XLSX file");
                    // Traitement supplémentaire spécifique au XLSX
                }
            }
        }
    }
}
```

### Voir aussi

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


