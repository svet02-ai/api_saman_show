# 🏟 Documentación API saman_show 


Esta en la API del proyecto saman_show, en el siguiente url:


Usando la librería request de python realizaran una petición GET a dicho URL el cual les devolverá un array de json (diccionario), dichos diccionarios tiene la siguiente estructura:

```
 {
  "events": [
        {
            "title": String,
            "type": Int (tipo de evento: [1]Musical, [2]Obra de Teatro),
            "synopsys": String ("Solo es de la obra de teatro"), 
            "bands": Int ("Cantidad de artistas que tocaran, Solo si es Musical"), 
            "cartel": [
                String (cantante/actores),
            ],
            "layout": {
                "general": [
                    Int (fila),
                    Int (columna)
                ],
                "vip": [
                    Int (fila),
                    Int (columna)
                ]
            },
            "prices" : [Float (precio general), Float (precio VIP)], 
            "date": "2022-04-01" (String (Fecha del evento año/mes/dia)
        },
     }
  ],
   "food_fair_inventory": [
    {
        "name": String (nombre de la comida),
        "price": Float (precio de la comida),
        "amount": Int (cantidad de inventario),
        "type": Int ([1]Comida, [2]Bebida),
        "presentation": (Si es comida [1]Preparacion, [2]Empaque)
    }, 
  ] 
}
 
```

**Endpoint:** https://raw.githubusercontent.com/Algoritmos-y-Programacion/api_saman_show/main/api.json
