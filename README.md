# Typescript Client for Open Meteo

## Installation

```shell
npm install open-meteo-ts-client
```

## Usage

```javascript
import { WeatherForecastAPIsApi } from "open-meteo-ts-client";

const api = new WeatherForecastAPIsApi();
api.v1ForecastGet(lat, lon, ...).then(response => console.log(response.data));
```

## Publish

Pre-requisite: Docker

1. Update openapi.yaml file with latest release from https://github.com/open-meteo/open-meteo/blob/main/openapi.yml
2. ./scripts/build
3. cd dist && npm publish 

