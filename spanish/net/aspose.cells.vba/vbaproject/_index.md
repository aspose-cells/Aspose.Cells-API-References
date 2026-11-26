---
title: "Clase VbaProject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Vba.VbaProject. Representa el proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

Representa el proyecto VBA.

```csharp
public class VbaProject
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Obtiene los datos sin procesar del certificado si este proyecto VBA está firmado. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Obtiene y establece la codificación del proyecto VBA. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | Indica si este proyecto VBA está bloqueado para visualización. Si es verdadero, los códigos no podrían ser visibles. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**Obsolete.**) Indica si este proyecto VBA está bloqueado para visualización. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Indica si este proyecto VBA está protegido. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Indica si VBAcode está firmado o no. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Indica si la firma del proyecto VBA es válida o no. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Obtiene todos los objetos [`VbaModule`](../vbamodule/). |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Obtiene y establece el nombre del proyecto VBA. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Obtiene todas las referencias del proyecto VBA. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Copia el proyecto VBA de otro archivo. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Protege o desprotege este proyecto VBA. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Firma este proyecto VBA con una DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Valida la contraseña de protección. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Text;
    using System.Security.Cryptography.X509Certificates;

    public class VbaProjectDemo
    {
        public static void VbaProjectExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Estableciendo propiedades
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Comprobando propiedades de solo lectura.
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Añadiendo un módulo VBA.
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // Añadiendo una referencia al proyecto VBA.
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Protegiendo el proyecto VBA.
            vbaProject.Protect(true, "password");

            // Firmando el proyecto VBA.
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Guardando el archivo Excel
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


