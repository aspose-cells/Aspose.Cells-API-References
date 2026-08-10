---
title: "AbstractGlobalizationSettings Class"
linktitle: "AbstractGlobalizationSettings"
articleTitle: "AbstractGlobalizationSettings"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the globalization settings."
type: docs
weight: 40
url: /python-java/asposecells.api/abstractglobalizationsettings/
---

## AbstractGlobalizationSettings class

Represents the globalization settings.

## Methods

| Name | Description |
| --- | --- |
| [compare](#compare) | Compares two string values according to certain collation rules. |
| [getCollationKey](#getcollationkey) | Transforms the string into a comparable object according to certain collation rules. |

### compare(v1, v2, ignoreCase) {#compare}

Compares two string values according to certain collation rules.

| Parameter | Type | Description |
| --- | --- | --- |
| v1 | String | the first string |
| v2 | String | the second string |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:** Integer that indicates the lexical relationship between the two comparands

### getCollationKey(v, ignoreCase) {#getcollationkey}

Transforms the string into a comparable object according to certain collation rules.

| Parameter | Type | Description |
| --- | --- | --- |
| v | String | String value needs to be compared with others. |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:** Object can be used to compare or sort string values
