---
title: "PivotField.Group"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Автоматически группирует поле."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/group/
---
## Group() {#group}

Автоматически группировать поле.

```csharp
public bool Group()
```

### Примечания

Если поле содержит только пустые значения и дату/время, оно будет сгруппировано по месяцам. Если поле содержит только пустые значения и числа, оно будет сгруппировано по числам. В остальных случаях возвращается false без какой-либо группы.

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Group(PivotFieldGroupOptions) {#group_1}

Группирует поле сводки с параметрами.

```csharp
public bool Group(PivotFieldGroupOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | PivotFieldGroupOptions | Параметры настройки группировки полей сводной таблицы. |

### См. также

* class [PivotFieldGroupOptions](../../pivotfieldgroupoptions/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


