---
title: "OrderProcessOptions"
weight: 10
date: 2019-01-30T10:57:03.820Z
generated: true
---
<!-- This file was generated from the Vendure TypeScript source. Do not modify. Instead, re-run "generate-docs" -->


# OrderProcessOptions

{{< generation-info source="/server/src/config/vendure-config.ts">}}



### transtitions

{{< member-info kind="property" type="Partial&#60;Transitions&#60;T | OrderState&#62;&#62;" >}}

Define how the custom states fit in with the default order

### onTransitionStart

{{< member-info kind="method" type="(fromState: T, toState: T, data: { order: Order }) => boolean | Promise&#60;boolean&#62; | Observable&#60;boolean&#62; | void" >}}

Define logic to run before a state tranition takes place. Returning

### onTransitionEnd

{{< member-info kind="method" type="(fromState: T, toState: T, data: { order: Order }) => void" >}}

Define logic to run after a state transition has taken place.

### onError

{{< member-info kind="method" type="(fromState: T, toState: T, message: string) => void" >}}

Define a custom error handler function for transition errors.
