---
title: "Enumeración XAdESType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.DigitalSignatures.XAdESType. Tipo de Firma Electrónica Avanzada XML XAdES"
type: docs
url: /es/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

Tipo de Firma Electrónica Avanzada XML (XAdES).

```csharp
public enum XAdESType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | XAdES está desactivado. |
| XAdES | `1` | XAdES básico. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;
    using System.Security.Cryptography.X509Certificates;

    public class XAdESTypeDemo
    {
        public static void XAdESTypeExample()
        {
            // Directorio de origen
            string sourceDir = "path_to_source_directory";
            // Directorio de salida
            string outputDir = "path_to_output_directory";
            // Cargar el libro de trabajo
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // Definir la contraseña para el archivo PFX
            string password = "pfxPassword";
            // Ruta al archivo PFX
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Crear una firma digital
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // Establecer el tipo XAdES
            signature.XAdESType = XAdESType.XAdES;

            // Crear una colección de firmas digitales
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Establecer la firma digital en el libro de trabajo
            workbook.SetDigitalSignature(dsCollection);

            // Guardar el libro de trabajo con la firma digital
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Verificar la firma digital
            Workbook signedWorkbook = new Workbook(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
                Console.WriteLine($"XAdES Type: {ds.XAdESType}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


