---
title: "FileFormatInfo.IsEncrypted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FileFormatInfo. Devuelve verdadero si el documento está encriptado y requiere una contraseña para abrirse"
type: docs
url: /es/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Devuelve true si el documento está cifrado y requiere una contraseña para abrirse.

```csharp
public bool IsEncrypted { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Detectar formato de archivo de un archivo no encriptado
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // Detectar formato de archivo de un archivo encriptado
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // Cargar archivo encriptado con contraseña
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### Ver también

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


