---
title: "VbaProject.CertRawData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Obtiene los datos sin procesar del certificado si este proyecto VBA está firmado"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

Obtiene los datos sin procesar del certificado si este proyecto VBA está firmado.

```csharp
public byte[] CertRawData { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaProjectPropertyCertRawDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con proyecto VBA
            Workbook workbook = new Workbook();
            // No es necesario crear un nuevo VbaProject ya que Workbook ya tiene uno

            // Acceder al proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Verificar si el proyecto VBA está firmado
            if (vbaProject.IsSigned)
            {
                // Mostrar los datos sin procesar del certificado si está firmado
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // Ejemplo: Guardar los datos del certificado en un archivo si existe
                if (certData != null && certData.Length > 0)
                {
                    File.WriteAllBytes("VbaCertificate.cer", certData);
                    Console.WriteLine("Certificate saved to file.");
                }
            }
            else
            {
                Console.WriteLine("VBA Project is not signed. CertRawData is not available.");
            }

            // Escenario de ejemplo: Cargar un Workbook con proyecto VBA firmado
            string signedWorkbookPath = "SignedWithVba.xlsm";
            if (File.Exists(signedWorkbookPath))
            {
                Workbook signedWorkbook = new Workbook(signedWorkbookPath);
                VbaProject signedVbaProject = signedWorkbook.VbaProject;

                if (signedVbaProject.IsSigned)
                {
                    byte[] signedCertData = signedVbaProject.CertRawData;
                    Console.WriteLine("Loaded workbook's VBA certificate data length: " + 
                        (signedCertData != null ? signedCertData.Length : 0));
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


