---
title: "GridWorksheet.FilterString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridWorksheet. Устанавливает фильтр для столбца. Обратите внимание, что необходимо вызвать AddAutoFilter перед вызовом filterString. Строка критериев фильтра. Обратите внимание, что мы используем запятую как разделитель, поэтому значение ячейки, которое вы хотите отфильтровать, не должно содержать запятую. filterString10123456 означает, что столбец 10 должен содержать 123 или 456. filterString10123 означает, что столбец 10 должен содержать 123. Индекс столбца разделяется запятой, например 123456789 или abc."
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridworksheet/filterstring/
---
## GridWorksheet.FilterString method

Устанавливает фильтр для столбца. Обратите внимание, что перед вызовом filterString необходимо вызвать AddAutoFilter. Строка критериев фильтра. Обратите внимание, что в качестве разделителя используется запятая-&gt;"," , поэтому значение ячейки, которое вы хотите отфильтровать, не должно содержать запятую. filterString(10,"123,456") означает, что столбец 10 должен содержать 123 или 456, filterString(10,"123") означает, что столбец 10 должен содержать 123. Индекс столбца разделяется запятой, например 123,456,789 или abc.

```csharp
public void FilterString(int column, string criteria)
```

### См. также

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


