---
layout: page
permalink: /travel/
title: Travel
description: 
nav: false
nav_order: 6
map: true
---

I have been lucky to had the opportunity to attend conferences in so many amazing places:

```geojson
{"type":"FeatureCollection","features":[{"type":"Feature","properties":{"University of Oxford":"Young Researchers in Algebraic Number Theory","University of Arizona":"Arizona Winter School","Universidad de Sevilla":"RGAS School of Singularities","University of Nottingham":"Inaugural Conference of the UK Algebraic Geometry Network","University of Cambridge":"Young Researchers in Algebraic Number Theory","West Lexham":"Queer in Number Theory and Geometry"},"geometry":{"coordinates":[-1.2618500000021982,51.76008282885644],"type":"Point"},"id":0},{"type":"Feature","properties":{"University of Arizona":"","University of Oxford":"","Universidad de Sevilla":""},"geometry":{"coordinates":[-110.9532087288355,32.22941638640397],"type":"Point"},"id":1},{"type":"Feature","properties":{"Universidad de Sevilla":""},"geometry":{"coordinates":[-5.9873032711618634,37.359047263899924],"type":"Point"},"id":2},{"type":"Feature","properties":{"University of Nottingham":""},"geometry":{"coordinates":[-1.1922857288347188,52.94054576716863],"type":"Point"},"id":3},{"type":"Feature","properties":{"University of Cambridge":""},"geometry":{"coordinates":[0.10292962069397049,52.20961825190716],"type":"Point"},"id":4},{"type":"Feature","properties":{"West Lexham":""},"geometry":{"coordinates":[0.7267890182767189,52.72119333656332],"type":"Point"},"id":5}]}```



This is an example post with some [geojson](https://geojson.org/) code. The support is provided thanks to [Leaflet](https://leafletjs.com/). To create your own visualization, go to [geojson.io](https://geojson.io/).

````markdown
```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {},
      "geometry": {
        "coordinates": [
          [
            [
              -60.11363029935569,
              -2.904625022183211
            ],
            [
              -60.11363029935569,
              -3.162613728707967
            ],
            [
              -59.820894493858034,
              -3.162613728707967
            ],
            [
              -59.820894493858034,
              -2.904625022183211
            ],
            [
              -60.11363029935569,
              -2.904625022183211
            ]
          ]
        ],
        "type": "Polygon"
      }
    }
  ]
}
```
````

Which generates:

```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {},
      "geometry": {
        "coordinates": [
          [
            [
              -60.11363029935569,
              -2.904625022183211
            ],
            [
              -60.11363029935569,
              -3.162613728707967
            ],
            [
              -59.820894493858034,
              -3.162613728707967
            ],
            [
              -59.820894493858034,
              -2.904625022183211
            ],
            [
              -60.11363029935569,
              -2.904625022183211
            ]
          ]
        ],
        "type": "Polygon"
      }
    }
  ]
}
```