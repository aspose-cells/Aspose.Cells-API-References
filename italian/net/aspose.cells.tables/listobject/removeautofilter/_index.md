---
title: "ListObject.RemoveAutoFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Rimuove il filtro automatico applicato a questa tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/removeautofilter/
---
## ListObject.RemoveAutoFilter method

Rimuove il filtro automatico applicato a questa tabella.

```csharp
public void RemoveAutoFilter()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Popola dati di esempio (con riga di intestazione)
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("Alice");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Bob");
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B4"].PutValue("Charlie");

            try
            {
                // Aggiungi un ListObject (tabella) che include un filtro automatico per impostazione predefinita
                int listIndex = sheet.ListObjects.Add("A1", "B4", true);
                ListObject listObj = sheet.ListObjects[listIndex];

                // Opzionale: applica un filtro per dimostrare che un filtro esiste
                listObj.Filter();

                // Rimuovi il filtro automatico dal ListObject
                listObj.RemoveAutoFilter();

                Console.WriteLine("RemoveAutoFilter called successfully.");
                
                // Salva la cartella di lavoro per verificare le modifiche
                workbook.Save("RemoveAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during RemoveAutoFilter operation: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


