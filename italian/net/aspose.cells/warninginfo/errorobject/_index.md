---
title: "WarningInfo.ErrorObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WarningInfo. L'oggetto di errore"
type: docs
url: /it/net/aspose.cells/warninginfo/errorobject/
---
## WarningInfo.ErrorObject property

L'oggetto errore.

```csharp
public object ErrorObject { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyErrorObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int nameIndex = workbook.Worksheets.Names.Add("MyName");
            workbook.Worksheets.Names[nameIndex].RefersTo = "=Sheet1!$A$1";
            workbook.Settings.WarningCallback = new NameWarningCallback(workbook);
            
            // Genera un conflitto di nomi copiando un foglio di lavoro con i nomi
            workbook.Worksheets.AddCopy(sheet.Name);
        }

        private class NameWarningCallback : IWarningCallback
        {
            private readonly Workbook _workbook;
            
            public NameWarningCallback(Workbook workbook) => _workbook = workbook;

            public void Warning(WarningInfo warningInfo)
            {
                if (warningInfo.Type == ExceptionType.DefinedName)
                {
                    int originalIndex = (int)warningInfo.ErrorObject;
                    Name originalName = _workbook.Worksheets.Names[originalIndex];
                    
                    int newIndex = _workbook.Worksheets.Names.Add(originalName.Text + "_Copy");
                    _workbook.Worksheets.Names[newIndex].RefersTo = originalName.RefersTo;
                    
                    warningInfo.CorrectedObject = newIndex;
                }
            }
        }
    }
}
```

### Vedi anche

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


