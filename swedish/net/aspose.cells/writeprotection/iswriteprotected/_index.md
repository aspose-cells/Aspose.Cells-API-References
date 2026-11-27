---
title: "WriteProtection.IsWriteProtected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WriteProtection-egenskapen. Anger om den här arbetsboken är skrivskyddad"
type: docs
url: /sv/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Anger om den här arbetsboken är skrivskyddad.

```csharp
public bool IsWriteProtected { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aktivera skrivskydd med lösenord
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Kontrollera om arbetsboken är skrivskyddad
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // Validera lösenordet
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // Spara arbetsboken
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera skyddet
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // Kontrollera skyddstatusen igen
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Se även

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


