---
title: "Klass AbstractLowCodeProtectionProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.AbstractLowCodeProtectionProvider-klass. Implementation för att tillhandahålla skyddsinställningar"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/
---
## AbstractLowCodeProtectionProvider class

Implementering för att tillhandahålla skyddsinställningar.

```csharp
public class AbstractLowCodeProtectionProvider
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [AbstractLowCodeProtectionProvider](abstractlowcodeprotectionprovider/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [GetOpenPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/)() | Hämtar lösenordet för att öppna kalkylbladsfilen. |
| virtual [GetWorkbookPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/)() | Hämtar lösenordet för att skydda arbetsboken med angiven skyddstyp. |
| virtual [GetWorkbookProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/)() | Hämtar skyddstypen för att skydda arbetsboken. |
| virtual [GetWorksheetPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/)(string) | Hämtar lösenordet för att skydda det angivna kalkylbladet. |
| virtual [GetWorksheetProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/)(string) | Hämtar skyddstypen för att skydda det angivna kalkylbladet. |
| virtual [GetWritePassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/)() | Hämtar lösenordet för att ändra kalkylbladsfilen. |

### Exempel

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
            // Skapa en ny arbetsbok och lägg till testkalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("AuditReport");

            // Skapa en instans av anpassad skyddsleverantör
            var protectionProvider = new CustomProtectionProvider();

            // Applicera arbetsboks-skydd
            workbook.Protect(
                protectionProvider.GetWorkbookProtectionType(),
                protectionProvider.GetWorkbookPassword()
            );

            // Applicera skydd på alla arbetsblad
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                worksheet.Protect(
                    protectionProvider.GetWorksheetProtectionType(worksheet.Name),
                    null,  // Add null for oldPassword parameter
                    protectionProvider.GetWorksheetPassword(worksheet.Name)
                );
            }

            // Ange lösenord för filåtkomst
            workbook.Settings.Password = protectionProvider.GetOpenPassword();
            workbook.Settings.WriteProtection.Password = protectionProvider.GetWritePassword();

            // Spara skyddad arbetsbok
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

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


