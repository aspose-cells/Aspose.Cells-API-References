---
title: "FileFormatUtil.DetectFileFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FileFormatUtil. Détecte et retourne les informations sur le format d'un fichier Excel stocké dans un stream"
type: docs
url: /fr/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Détecte et renvoie les informations sur le format d'un Excel stocké dans un flux.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream |  |

### Valeur de retour

Un objet [`FileFormatInfo`](../../fileformatinfo/) qui contient les informations détectées.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FileFormatUtilMethodDetectFileFormatWithStreamDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Préparer un MemoryStream avec les données du classeur
            using (MemoryStream stream = new MemoryStream())
            {
                // Enregistrer le classeur dans le flux au format XLSX
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // Détecter le format de fichier depuis le flux
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // Afficher les résultats de détection
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // Enregistrer le classeur original pour vérification
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Détecte et renvoie les informations sur le format d'un Excel stocké dans un flux.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| mot de passe | String | Le mot de passe pour les fichiers ooxml chiffrés. |

### Valeur de retour

Un objet [`FileFormatInfo`](../../fileformatinfo/) qui contient les informations détectées.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStreamStringDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xlsx";
            
            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
                Console.WriteLine("Is password valid: " + FileFormatUtil.VerifyPassword(stream, "test"));
            }

            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
            }
        }
    }
}
```

### Voir aussi

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Détecte et renvoie les informations sur le format d'un Excel stocké dans un fichier.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | String | Le chemin du fichier. |

### Valeur de retour

Un objet [`FileFormatInfo`](../../fileformatinfo/) qui contient les informations détectées.

### Remarques

Ne prend en charge que la vérification de certains fichiers avec une signature magique. S'il n'y a pas de signature magique, nous ne pouvons pas détecter précisément le format du fichier.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            
            Console.WriteLine("Load Format: " + info.LoadFormat);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(info.FileFormatType);
            LoadFormat loadFormat = FileFormatUtil.SaveFormatToLoadFormat(saveFormat);
            
            Console.WriteLine("Save Format: " + saveFormat);
            Console.WriteLine("Load Format (converted): " + loadFormat);
        }
    }
}
```

### Voir aussi

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Détecte et renvoie les informations sur le format d'un Excel stocké dans un fichier.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | String | Le chemin du fichier. |
| mot de passe | String | Le mot de passe pour les fichiers ooxml chiffrés. |

### Valeur de retour

Un objet [`FileFormatInfo`](../../fileformatinfo/) qui contient les informations détectées.

### Remarques

Ne prend en charge que la vérification de certains fichiers avec une signature magique. S'il n'y a pas de signature magique, nous ne pouvons pas détecter précisément le format du fichier.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringStringDemo
    {
        public static void Run()
        {
            string sourcePath = @"..\..\..\Data\";
            
            // Détecter le format de fichier XLSX
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // Détecter le format de fichier DOCX
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### Voir aussi

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


