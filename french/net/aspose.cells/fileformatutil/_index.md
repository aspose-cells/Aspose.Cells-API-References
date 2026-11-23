---
title: "Classe FileFormatUtil"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FileFormatUtil. Fournit des méthodes utilitaires pour convertir les énumérations de format de fichier en chaînes ou en extensions de fichier et inversement"
type: docs
url: /fr/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

Fournit des méthodes utilitaires pour convertir les énumérations de format de fichier en chaînes ou en extensions de fichier et inversement.

```csharp
public class FileFormatUtil
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Détecte et renvoie les informations sur le format d'un Excel stocké dans un flux. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Détecte et renvoie les informations sur le format d'un Excel stocké dans un fichier. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Détecte et renvoie les informations sur le format d'un Excel stocké dans un flux. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Détecte et renvoie les informations sur le format d'un Excel stocké dans un fichier. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Convertit une extension de nom de fichier en valeur SaveFormat. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Conversion du format de fichier en format d'enregistrement. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Renvoie true si l'extension est .xlt, .xltX, .xltm,.ots. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Convertit une valeur d'énumération de format de chargement en extension de fichier. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Convertit une valeur LoadFormat en valeur SaveFormat si possible. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Convertit une valeur d'énumération de format d'enregistrement en extension de fichier. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Convertit une valeur SaveFormat en valeur LoadFormat si possible. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Détecte et renvoie les informations sur le format d'un Excel stocké dans un flux. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFileFormatUtilDemo
    {
        public static void Run()
        {
            string filePath = "example.xlt";
            
            // Détecter le format de fichier
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // Vérifier le format de fichier avec Workbook
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


