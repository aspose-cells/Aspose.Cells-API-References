---
title: "WorkbookSettings.Password"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Representerar lösenordet för kryptering av arbetsbokfilen"
type: docs
url: /sv/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Anger arbetsbokens filkrypteringslösenord.

```csharp
public string Password { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Öppna det första kalkylbladet och lägg till data
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // Ange lösenord för att skydda arbetsboken
            wb.Settings.Password = "xixi";
            
            // Spara arbetsboken
            wb.Save("output_with_password.ods");
            
            // Skapa laddningsalternativ med lösenord för att öppna den skyddade arbetsboken
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // Öppna den lösenordsskyddade arbetsboken
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // Verifiera data
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


