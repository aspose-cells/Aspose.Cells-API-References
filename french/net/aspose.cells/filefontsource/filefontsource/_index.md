---
title: "FileFontSource.FileFontSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur FileFontSource. Ctor"
type: docs
url: /fr/net/aspose.cells/filefontsource/filefontsource/
---
## FileFontSource constructor

Constructeur.

```csharp
public FileFontSource(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | String | chemin du fichier de police |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourceMethodCtorWithStringDemo
    {
        public static void Run()
        {
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);

            workbook.Save("FileFontSourceExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


