---
title: "LightCellsDataProvider.IsGatherString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataProvider‑Methode. Prüft, ob der aktuelle Zeichenkettenwert einer Zelle in einen globalen Pool gesammelt werden muss"
type: docs
url: /de/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Überprüft, ob der aktuelle Zeichenkettenwert der Zelle in einen globalen Pool aufgenommen werden muss.

```csharp
public bool IsGatherString()
```

### Rückgabewert

true, wenn der Zeichenkettenwert für die resultierende Datei in einen globalen Pool gesammelt werden muss.

### Hinweise

Das Sammeln von Zeichenkettenwerten ist nur dann vorteilhaft, wenn viele duplizierte Zeichenkettenwerte für die von dieser Implementierung bereitgestellten Zellen vorliegen. In diesem Fall spart das Sammeln von Zeichenketten erheblich Speicher und erzeugt eine kleinere Ergebnisdatei. Wenn es viele Zeichenkettenwerte für die von LightCellsDataProvider bereitgestellten Zellen gibt, aber nur wenige davon identisch sind, kostet das Sammeln von Zeichenketten mehr Speicher und Zeit und bietet keinen Vorteil für die Ergebnisdatei.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodIsGatherStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with IsGatherString implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly object[,] data = new object[3, 2]
            {
                { "Product", "Price" },
                { "Laptop", 1200.50 },
                { "Phone", 899.99 }
            };

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 3 ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString()
            {
                // Nur Zeichenketten für die Kopfzeile sammeln (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


