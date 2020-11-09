# React Basic World Map

Includes basic world map and continents.

## Demo

![demo](https://user-images.githubusercontent.com/41209531/98580338-dbbbec00-22d0-11eb-910a-5492cd52a84c.gif)

## Installation


```bash
npm install react-basic-world-map --save
```

## Usage

```react
<BasicWorldMap />
```

```react
<BasicWorldMap
    primaryColor="black"
    secondaryColor="gray"
/>
```

```react
const onClickMapLocation = (selected: ContinentItem) => {
    // do something
}

const continents = [
    { key: "africa", value: "Afrika" },
    { key: "south_america", value: "Güney Amerika" },
    { key: "europe", value: "Avrupa" },
    { key: "asia", value: "Asya" },
    { key: "america", value: "Amerika" },
    { key: "australia", value: "Okyanusya" }
]

<BasicWorldMap
    primaryColor="black"
    secondaryColor="gray"
    onClickMapContinent={onClickMapLocation}
    continents= {continents}
/>
```

## Props
```react
onClickMapContinent

primaryColor

secondaryColor

continents
```

## License
[ISC](https://opensource.org/licenses/ISC)