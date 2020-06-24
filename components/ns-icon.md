---
description: Icon component.
---

# ns-icon

## Introduction

> Icons are visual symbols used to represent functions, products and services.

Icons provide clarity to users reducing the cognitive load. Icons always supplement a single line of text and are not treated as a description. They are solid or outline a single colour.

## Usage

To see examples visit [Storybook](https://britishgas.co.uk/nucleus/demo/index.html?path=/story/ns-icon--gas).

{% embed url="https://codesandbox.io/s/github/britishgas-engineering/nucleus-examples/tree/master/demos/ns-icon" caption="" %}

```markup
<ns-icon type="gas"></ns-icon>
```

## Component Relationship

**Does it live in a panel?**  
No

**What layout classes can be used?**  
None

**Does it live inside other components?**  
`ns-cta`  
`ns-expander`  
`ns-inputter`  
`ns-tab`

**Atomic type**  
Atom

## Specification

| **Name** | Type |
| :--- | :--- |
| **Description** | The name of the icon |
| **Type** | string |
| **Default** | arrow |
| **Options** | appliance,appliance-outline,appliance-solid,arrow,arrow-left,arrow-right,bill,bill-outline,bill-solid,boiler,boiler-outline,boiler-solid,chevron,chevron-down,chevron-left,chevron-right,chevron-up,cross,download,electricity,electricity-outline,electricity-solid,gas,gas-outline,gas-solid,hive,home,home-outline,home-solid,loading,meter,meter-outline,meter-solid,minus,plus,protect,protect-outline,protect-solid,rewards,rewards-outline,rewards-solid,settings,tick,warning |
| **Notes** | Functioal icons like 'arrow' only have one version while products and services like 'gas' have an outline and solid versions where solid is the default |

| **Name** | Size |
| :--- | :--- |
| **Description** | The size of the icon |
| **Type** | string |
| **Default** | "" |
| **Options** | "", 1, 2, 3, 4, 5 |
| **Notes** | If you pass an empty size the icon will fill the parent element |

## Best practices

| 💚 Do's | 💔 Dont's |
| :--- | :--- |
| Use icons within the component | Create your own icons |
| Use this when building new Nucleus components | Add them as content |
| Use them in colours |  |
| Keep them small |  |

### Considerations of best practices

* Icons can be used as navigational elements as solid or outline single colour.
* If you want to use larger iconography have a look at ns-illustration.
* Use outline icons when... and solid icons when... .

## Feedback

* Do you have insights or concerns to share? You can raise an issue via [Github bugs](https://github.com/ConnectedHomes/nucleus/issues/new?assignees=&labels=Bug&template=a--bug-report.md&title=[bug]%20[ns-icon]).
* See all the issues already raised via [Github issues](https://github.com/connectedHomes/nucleus/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+label%3ABug+[ns-icon]).

💩 🎉 🦄 You can also contact the team on Slack on the `#product-nucleus` channel!

## Related links

* [ns-cta](https://docs.britishgas.design/components/ns-cta).
* [How to create icons guide](https://docs.britishgas.design/how-to/creating-icons).
* Guiding Customers with our icons and the difference between icons and illustrations in Brand Guidelines.
* If you wish to have us consider adding a new icon to the library please consult Brand Visual Identity managers.
