---
title: "Classe AbstractLowCodeProtectionProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.AbstractLowCodeProtectionProvider. Implementazione per fornire impostazioni di protezione"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/
---
## AbstractLowCodeProtectionProvider class

Implementazione per fornire impostazioni di protezione

```csharp
public class AbstractLowCodeProtectionProvider
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AbstractLowCodeProtectionProvider](abstractlowcodeprotectionprovider/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [GetOpenPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/)() | Ottiene la password per aprire il file di foglio di calcolo. |
| virtual [GetWorkbookPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/)() | Ottiene la password per proteggere la cartella di lavoro con il tipo di protezione specificato. |
| virtual [GetWorkbookProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/)() | Ottiene il tipo di protezione per proteggere la cartella di lavoro. |
| virtual [GetWorksheetPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/)(string) | Ottiene la password per proteggere il foglio di lavoro specificato. |
| virtual [GetWorksheetProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/)(string) | Ottiene il tipo di protezione per proteggere il foglio di lavoro specificato. |
| virtual [GetWritePassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/)() | Ottiene la password per modificare il file di foglio di calcolo. |

### Esempi

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
            // Crea una nuova cartella di lavoro e aggiungi fogli di lavoro di prova
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("AuditReport");

            // Crea un'istanza del provider di protezione personalizzato
            var protectionProvider = new CustomProtectionProvider();

            // Applica la protezione della cartella di lavoro
            workbook.Protect(
                protectionProvider.GetWorkbookProtectionType(),
                protectionProvider.GetWorkbookPassword()
            );

            // Applica la protezione a tutti i fogli di lavoro
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                worksheet.Protect(
                    protectionProvider.GetWorksheetProtectionType(worksheet.Name),
                    null,  // Add null for oldPassword parameter
                    protectionProvider.GetWorksheetPassword(worksheet.Name)
                );
            }

            // Imposta le password di accesso al file
            workbook.Settings.Password = protectionProvider.GetOpenPassword();
            workbook.Settings.WriteProtection.Password = protectionProvider.GetWritePassword();

            // Salva la cartella di lavoro protetta
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

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


