# Pl-Labeled-container
Контейнер с подписью позволяет комбинировать другой компонент с подписью в общий элемент

<pl-labeled-container label="Текст подписи"></pl-labeled-container>

## Examples

### Orientation
Используйте `orientation` для изменения расположения текста
<pl-labeled-container label="horizontal orientation" orientation="horizontal" label-width="130">
    <button>Button</button>
</pl-labeled-container>
<br>
<pl-labeled-container label="vertical orientation">
    <button>Button</button>
</pl-labeled-container>

<details>
    <summary>html</summary>

    <pl-labeled-container label="horizontal orientation" orientation="horizontal" label-width="130">
        <button>Button</button>
    </pl-labeled-container>

    <pl-labeled-container label="vertical orientation">
        <button>Button</button>
    </pl-labeled-container>
</details>

### ContentWidth
Используйте `сontentWidth`для того что бы указать ширину контейнера

<pl-labeled-container label="content-width=100" orientation="horizontal" label-width="120" content-width="100">
    <button style="width: 100%">Button</button>
</pl-labeled-container>
<br>
<pl-labeled-container label="content-width=200" orientation="horizontal" label-width="120" content-width="200">
    <button style="width: 100%">Button</button>
</pl-labeled-container>

<details>
    <summary>html</summary>

    <pl-labeled-container label="content-width=100" orientation="horizontal" label-width="120" content-width="100">
        <button style="width: 100%">Button</button>
    </pl-labeled-container>

    <pl-labeled-container label="content-width=200" orientation="horizontal" label-width="120" content-width="200">
        <button style="width: 100%">Button</button>
    </pl-labeled-container>
</details>

### labelWidth
Используйте `labelWidth`для того что бы указать ширину подписи

<pl-labeled-container label="labelWidth=100" orientation="horizontal" label-width="120">
    <button>Button</button>
</pl-labeled-container>
<br>
<pl-labeled-container label="labelWidth=80" orientation="horizontal" label-width="90">
    <button>Button</button>
</pl-labeled-container>

<details>
    <summary>html</summary>

    <pl-labeled-container label="labelWidth=100" orientation="horizontal" label-width="120">
        <button>Button</button>
    </pl-labeled-container>

    <pl-labeled-container label="labelWidth=80" orientation="horizontal" label-width="90">
        <button>Button</button>
    </pl-labeled-container>
</details>

### Slots
Используйте `label-prefix` или `label-suffix` для того что бы добавить иконку к подписи
<pl-labeled-container label="label-prefix" orientation="horizontal">
    <pl-icon slot="label-prefix" variant="primary" iconset="pl-default" size="16" icon="settings"></pl-icon>
</pl-labeled-container>
<br>
<pl-labeled-container label="label-suffix" label-width="80" orientation="horizontal">
    <pl-icon slot="label-suffix" variant="primary" iconset="pl-default" size="16" icon="settings"></pl-icon>
</pl-labeled-container>

<details>
    <summary>html</summary>

    <pl-labeled-container label="label-prefix" orientation="horizontal">
        <pl-icon slot="label-prefix" variant="primary" iconset="pl-default" size="16" icon="settings"></pl-icon>
    </pl-labeled-container>

    <pl-labeled-container label="label-suffix" label-width="80" orientation="horizontal">
        <pl-icon slot="label-suffix" variant="primary" iconset="pl-default" size="16" icon="settings"></pl-icon>
    </pl-labeled-container>
</details>

## Properties

| Name  | Description  | ReflectsToAttribute | Type | Default
|---|---|:----:|---|:---:|
| `label` | Метка  | - | string |  (empty) 
| `orientation` | Расположение подписи относительно текстового поля | - | `horizontal \| vertical` | `vertical`
| `contentWidth` | Значение ширины поля ввода<br> *По умолчанию задается ширина в 240px*  |  + | `number` | (empty)
| `labelWidth` | Значение ширны метки поля<br> *По умолчанию задается ширина в 240px*  |  + | `number` | (empty)


## Slots

| Name  | Description  
|---|---
| (default) | Слот для дочернего компонента контейнера
| `label-prefix` | Слот для префикса метки, значки располагаются перед меткой
| `label-suffix` | Слот для суфикс метки, значки располагаются после меткой