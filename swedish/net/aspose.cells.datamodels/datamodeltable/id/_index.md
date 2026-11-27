---
title: "Visa det aktuella Id‑värdet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Obs: Id‑egenskapen är skrivskyddad, så vi kan inte sätta den"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

Hämtar id för datamodelltabellen.

```csharp
public string Id { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // Skapa ett ListObject (tabell)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Detta demonstrerar hur man får åtkomst till och använder det befintliga Id:t
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Exempel på användning: Jämför tabell‑ID:n när du arbetar med flera tabeller
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // DataModelTable.Name
            // DataModelTable‑egenskap. Hämtar namnet på datamodelltabellen

            // DataModelTable.ConnectionName
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // Spara arbetsboken
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


