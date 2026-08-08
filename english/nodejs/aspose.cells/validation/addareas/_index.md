---
title: "Validation.addAreas"
linktitle: "addAreas"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Applies the validation to given areas."
type: docs
weight: 30
url: /nodejs/aspose.cells/validation/addareas/
---

## addAreas(areas, checkIntersection, checkEdge)

Applies the validation to given areas. In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.

| Parameter | Type | Description |
| --- | --- | --- |
| areas | Array ofCellArea | The areas. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that all the added areas do not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if one of given areas will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that no one of those added areas is the top-left, this parameter can be set as false for performance consideration. |
