---
title: "Worksheet.FilterString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet method. Устанавливает фильтр для столбца. Примечание: мы должны вызвать AddAutoFilter перед вызовом filterString. Строка критериев фильтра. Примечание: мы используем запятую как разделитель, поэтому значение ячейки, которое вы хотите отфильтровать, не должно содержать запятую. filterString10123456 означает, что столбец 10 должен содержать 123 или 456. filterString10123 означает, что столбец 10 должен содержать 123, значение разделено запятой, например 123456789 или abc."
type: docs
url: /ru/net/aspose.cells.griddesktop/worksheet/filterstring/
---
## Worksheet.FilterString method

Устанавливает фильтр для столбца. Обратите внимание, что необходимо вызвать AddAutoFilter перед вызовом filterString. Строка критериев фильтра. Обратите внимание, что мы используем запятую -> \",\" в качестве разделителя, поэтому значение ячейки, которое вы хотите отфильтровать, не должно содержать запятую. filterString(10,\"123,456\") означает, что столбец 10 должен содержать 123 или 456, filterString(10,\"123\") означает, что столбец 10 должен содержать значение 123, разделённое запятыми, например 123,456,789 или abc

```csharp
public void FilterString(int column, string criteria)
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


