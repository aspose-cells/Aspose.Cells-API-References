---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FileFormatUtil. Conversion du format de fichier en format d'enregistrement"
type: docs
url: /fr/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Conversion du format de fichier en format d'enregistrement.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| format | FileFormatType | Le type de format de fichier. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // Obtenez le type de format de fichier du classeur
            FileFormatType originalFormat = workbook.FileFormat;

            // Convertir FileFormatType en SaveFormat
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // Enregistrez le classeur en utilisant le SaveFormat converti
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


