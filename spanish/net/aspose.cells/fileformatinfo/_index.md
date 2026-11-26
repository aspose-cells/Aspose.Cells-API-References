---
title: "Clase FileFormatInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FileFormatInfo. Contiene datos devueltos por los métodos de detección de formato de archivo de FileFormatUtil"
type: docs
url: /es/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

Contiene datos devueltos por los métodos de detección de formato de archivo de [`FileFormatUtil`](../fileformatutil/).

```csharp
public class FileFormatInfo
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Obtiene el formato de archivo detectado. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Devuelve true si el documento está cifrado y requiere una contraseña para abrirse. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Indica si el archivo está protegido por Microsoft Rights Management Server. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Obtiene el formato de carga detectado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // Cargue un archivo de muestra para detectar su formato
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Muestre la información del formato de archivo
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // Guarde la información en un archivo de texto
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

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


