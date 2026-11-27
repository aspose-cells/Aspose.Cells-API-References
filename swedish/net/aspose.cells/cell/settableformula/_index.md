---
title: "Cell.SetTableFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Skapa tvåvariabels datatabell för angivet område med start från denna cell"
type: docs
url: /sv/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Skapa en tvåvariabels datatabell för det angivna området med start från den här cellen.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |
| rowInputCell | String | radens inmatningscell |
| columnInputCell | String | kolumnens inmatningscell |
| värden | Object[][] | värden för celler i tabellformelområdet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // Målcellen där tabellformeln kommer att sättas
            Cell targetCell = worksheet.Cells["C3"];

            // Förbered parametrar för SetTableFormula
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Sätt tabellformeln på målcellen
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Beräkna arbetsbokens formler för att uppdatera resultat
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Skapa en envariabels datatabell för det angivna området med start från den här cellen.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |
| inputCell | String | indatacellen |
| isRowInput | Boolean | Anger om indata cellen är en radindata cell (true) eller en kolumnindata cell (false). |
| värden | Object[][] | värden för celler i tabellformelområdet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // Förbered parametrar för SetTableFormula
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // Hämta målcellen för datatabellen (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // Anropa SetTableFormula med räntevariationer
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // Beräkna formler för att uppdatera tabellresultat
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Skapa en tvåvariabels datatabell för det angivna området med start från den här cellen.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |
| rowIndexOfRowInputCell | Int32 | radindex för radindata cellen |
| columnIndexOfRowInputCell | Int32 | kolumnindex för radindata cellen |
| rowIndexOfColumnInputCell | Int32 | radindex för kolumnindata cellen |
| columnIndexOfColumnInputCell | Int32 | kolumnindex för kolumnindata cellen |
| värden | Object[][] | värden för celler i tabellformelområdet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // Förbered indata värden för datatabellen (räntor och lånebelopp)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // Sätt tabellformeln med 3x3 datatabelldimensioner och indata cellförskjutningar
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Skapa en envariabels datatabell för det angivna området med start från den här cellen.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |
| rowIndexOfInputCell | Int32 | radindex för indata cellen |
| columnIndexOfInputCell | Int32 | kolumnindex för indata cellen |
| isRowInput | Boolean | Anger om indata cellen är en radindata cell (true) eller en kolumnindata cell (false). |
| värden | Object[][] | värden för celler i tabellformelområdet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // Skapa exempeldataarray för tabellformelparametrar
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Hämta målcell för att tillämpa tabellformel
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // Ställ in tabellformel med: 
                // 3 rader, 2 kolumner, inmatningscell vid A1 (0,0), 
                // radinmatningstyp och exempelvärden
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


