---
title: NodeIterator.referenceNode
slug: Web/API/NodeIterator/referenceNode
page-type: web-api-instance-property
tags:
  - API
  - DOM
  - Experimental
  - NodeIterator
  - Property
browser-compat: api.NodeIterator.referenceNode
---
{{APIRef("DOM")}}{{ SeeCompatTable }}

The **`NodeIterator.referenceNode`** read-only returns the
{{domxref("Node")}} to which the iterator is anchored; as new nodes are inserted, the
iterator remains anchored to the reference node as specified by this property.

## Value

A {{domxref("Node")}}.

## Examples

```js
var nodeIterator = document.createNodeIterator(
    document.body,
    NodeFilter.SHOW_ELEMENT,
    { acceptNode: function(node) { return NodeFilter.FILTER_ACCEPT; } }
);
node = nodeIterator.referenceNode;
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The interface it belongs to: {{domxref("NodeIterator")}}
