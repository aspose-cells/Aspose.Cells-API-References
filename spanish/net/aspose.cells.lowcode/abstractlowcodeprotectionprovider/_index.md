---
title: "Clase AbstractLowCodeProtectionProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.AbstractLowCodeProtectionProvider. Implementación para proporcionar configuraciones de protección"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/
---
## AbstractLowCodeProtectionProvider class

Implementación para proporcionar configuraciones de protección

```csharp
public class AbstractLowCodeProtectionProvider
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AbstractLowCodeProtectionProvider](abstractlowcodeprotectionprovider/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [GetOpenPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/)() | Obtiene la contraseña para abrir el archivo de hoja de cálculo. |
| virtual [GetWorkbookPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/)() | Obtiene la contraseña para proteger el libro de trabajo con el tipo de protección especificado. |
| virtual [GetWorkbookProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/)() | Obtiene el tipo de protección para proteger el libro de trabajo. |
| virtual [GetWorksheetPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/)(string) | Obtiene la contraseña para proteger la hoja de cálculo especificada. |
| virtual [GetWorksheetProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/)(string) | Obtiene el tipo de protección para proteger la hoja de cálculo especificada. |
| virtual [GetWritePassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/)() | Obtiene la contraseña para modificar el archivo de hoja de cálculo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeProtectionProviderDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo y agrega hojas de cálculo de prueba
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("AuditReport");

            // Crea una instancia del proveedor de protección personalizado
            var protectionProvider = new CustomProtectionProvider();

            // Aplica la protección al libro de trabajo
            workbook.Protect(
                protectionProvider.GetWorkbookProtectionType(),
                protectionProvider.GetWorkbookPassword()
            );

            // Aplica la protección a todas las hojas de cálculo
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                worksheet.Protect(
                    protectionProvider.GetWorksheetProtectionType(worksheet.Name),
                    null,  // Add null for oldPassword parameter
                    protectionProvider.GetWorksheetPassword(worksheet.Name)
                );
            }

            // Establece contraseñas de acceso al archivo
            workbook.Settings.Password = protectionProvider.GetOpenPassword();
            workbook.Settings.WriteProtection.Password = protectionProvider.GetWritePassword();

            // Guarda el libro de trabajo protegido
            workbook.Save("AbstractLowCodeProtectionProviderDemo.xlsx");
        }
    }

    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword() => "SecureOpen123";
        public override string GetWritePassword() => "EditPermission456";
        public override string GetWorkbookPassword() => "WorkbookLock789";
        
        public override ProtectionType GetWorkbookProtectionType() => 
            ProtectionType.Windows;  // Prevent window structure changes

        public override string GetWorksheetPassword(string sheetName) => 
            $"SheetLock_{sheetName}";  // Dynamic password per sheet

        public override ProtectionType GetWorksheetProtectionType(string sheetName) => 
            ProtectionType.Contents;  // Protect cell contents
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


