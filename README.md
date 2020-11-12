# React Basic World Map

Includes basic svg world map and continents.

## Demo

![demo](https://user-images.githubusercontent.com/41209531/98580338-dbbbec00-22d0-11eb-910a-5492cd52a84c.gif)

## Installation


```bash
npm install react-basic-world-map --save
```

## Usage

```js
import BasicWorldMap from 'react-basic-world-map';

<BasicWorldMap />
```

```jsx
import BasicWorldMap from 'react-basic-world-map';

<BasicWorldMap
    primaryColor="black"
    secondaryColor="gray"
/>
```

## Full Usage

```jsx
import React from 'react';
import BasicWorldMap from 'react-basic-world-map';

export default function App() {

    const onClickMapLocation = (selectedContinent: ContinentItem) => {
        // do something
    }

    const continents: ContinentItem[] = [
        { key: "africa", value: "Afrika" },
        { key: "south_america", value: "Güney Amerika" },
        { key: "europe", value: "Avrupa" },
        { key: "asia", value: "Asya" },
        { key: "america", value: "Amerika" },
        { key: "australia", value: "Okyanusya" }
    ]

    return (
        <BasicWorldMap
            primaryColor="black"
            secondaryColor="gray"
            onClickMapContinent={onClickMapLocation}
            continents= {continents}
        />
    )
}
```

## Props

|Property                |Type                          |
|----------------|-------------------------------|
|primaryColor    |`string`            |
|seondaryColor   |`string`            |
|onClickMapContinent |`function`|
|continents |`array`|

## License
[ISC](https://opensource.org/licenses/ISC)