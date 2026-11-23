---
title: "Classe FileFormatInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FileFormatInfo. Contient les données renvoyées par les méthodes de détection de format de fichier de FileFormatUtil"
type: docs
url: /fr/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

Contient les données renvoyées par les méthodes de détection du format de fichier de [`FileFormatUtil`](../fileformatutil/).

```csharp
public class FileFormatInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Obtient le format de fichier détecté. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Renvoie true si le document est chiffré et nécessite un mot de passe pour l'ouvrir. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Indique si le fichier est protégé par Microsoft Rights Management Server. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Obtient le format de chargement détecté. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // Chargez un fichier d'exemple pour détecter son format
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Affiche les informations du format de fichier
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // Enregistrez les informations dans un fichier texte
            string outputFilePath = "FileFormatInfo.txt";
            using (System.IO.StreamWriter writer = new System.IO.StreamWriter(outputFilePath))
            {
                writer.WriteLine("File Format Information:");
                writer.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
                writer.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
                writer.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
                writer.WriteLine($"Load Format: {fileInfo.LoadFormat}");
            }

            Console.WriteLine($"File format information saved to {outputFilePath}");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


