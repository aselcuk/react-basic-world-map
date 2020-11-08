# React Basic World Map

Includes basic world map and continents.

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
    onClickMapContinent={onClickMapLocation}
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
onClickMapContinent(function(selectedItem){})

primaryColor

secondaryColor

continents
```

## License
[ISC](https://opensource.org/licenses/ISC)