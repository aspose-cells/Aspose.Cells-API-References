---
title: "FindOptions.SearchNext"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions‑egenskap. Sökordning. True söker nästa. False söker föregående"
type: docs
url: /sv/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

Sökordning. True: sök nästa. False: sök föregående.

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället FindOptions.SearchBackward‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan november 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // Skapa sökalternativ
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // Demonstrera SearchNext‑egenskapen (föråldrad, men visas för demonstration)
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // Sök framåt (standardbeteende)
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // Sök bakåt
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // Spara arbetsboken
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


