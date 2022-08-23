# DPF-EC | DPF-INDEX | DPF-INDEX-EC


**Objetivo General:**

- Plataforma de monitorizacion de tasas para inversiones a plazo fijo. 

- Permite comparar tazas entre instituciones financieras y elegir una con la tasa mas alta y una mejor inversion. 

La idea es  hacer algo parecido a [coinbase](https://www.coinbase.com/), [bitstamp](https://www.bitstamp.net/), [coincodex](https://coincodex.com/), [WebAnalysis](https://awebanalysis.com/es/crypto-currencies-monitor-price/), pero con Inversiones a plazo fijo en instituciones financieras del Ecuador.


## Disclaimer | Descargo de responsabilidad

> Esta plataforma es realizada con fines practicos y educativos, asi que la informacion mostrada puede no ser *exacta*. No confiar totalmente en la veracidad de la informacion mostrada, tomelo solo como una herramienta o resumen que ayudara en la investigacion y cotizcion de las tasas en inversiones en las instituciones financieras. Se recomienda que haga su propia investigacion y cotizacion mas detallada en cada institucion.


## Caracteristicas | Roadmap

- [ ] Un Cotizador general segun la tasa y plazos.
- [ ] Una vista en forma de tabla de un listado de las instituciones financieras con la mejor taza segun un plazo escogido en orden Ascendente.

  ![image](https://user-images.githubusercontent.com/11642622/186201685-371798c4-2da6-441f-99d5-6ab2b8eaff49.png)


- [ ] Una vista de un grafico que muestre las instituciones segun la tasa parecido a esto

  ![image](https://user-images.githubusercontent.com/11642622/186197363-281b11f7-0e4d-4e18-a976-58079e1b9149.png)


- [ ] Un proceso automatico de web scraping que obtenga informacion de paginas web de las instituciones financieras.

**Esquema Ejemplo de la informacion a generar:**
  
    ```json
    
    "FinancialCompanies": {
     "Top_Fees_Financial_Companies": [
        {
        "id":"1", 
        "name": "Jardin Azuayo",
        "rating": "AA",
        "last_update_date": "12/08/2022",
        "taxes":"-2%",
        "min_amount": "100",
        "period fees": [
             {
               "days_bt": "30-59",
               "fee": "5,65%"
             },
             {
               "days_bt": "60-89",
               "fee": "5,90%"
             },
             {
               "days_bt": "90-179",
               "fee": "6,15%"
             },
             {
               "days_bt": "180-269",
               "fee": "6,65%"
             },
             {
               "days_bt": "270-359",
               "fee": "6,90%"
             },
             {
               "days_bt": "360-9999",
               "fee": "7,90%"
             }
          ],                       
        "min_fee": "5,65%",
        "max_fee": "7,90%",
        "logo": "https://imagen-example.jpg",
        "product_name": "'CDP' | 'Poliza' | 'DPF' | 'Inversion'",
        "web": "https://pagina-banco.com"
        },
        {
          "id":"2", 
          "name": "JEP",
          "rating": "AA",
          "last_update_date": "12/08/2022",
          "taxes":"-2%"
          "min_amount": "100",
          "period fees": [
               {
                 "days_bt": "30-59",
                 "fee": "5,00%"
               },
               {
                 "days_bt": "60-89",
                 "fee": "5,25%"
               },
               {
                 "days_bt": "90-179",
                 "fee": "5,75%"
               },
               {
                 "days_bt": "180-269",
                 "fee": "6,50%"
               },
               {
                 "days_bt": "270-359",
                 "fee": "7,00%"
               },
               {
                 "days_bt": "360-9999",
                 "fee": "8,00%"
               }
            ],          
          "min_fee": "5,00%",
          "max_fee": "8,00%",
          "logo": "https://imagen-example.jpg",
          "product_name": "'CDP' | 'Poliza' | 'DPF' | 'Inversion'",
          "web": "https://pagina-banco.com"
        }
      ],
      "source": "dpf-ec.com",
      "Time": "Aug 2022",
      "Author": "Richard Palacios"
      "Portfolio": "https://richardpalaciosg.dev"
    }  
    ```
  ** Ejemplo de la informacion de tazas a obtener** de cada institucion, seran por plazos para poder hacer un simulador, cotizador, etc
   
  > Se debe considerar que los intereses mensuales están sujetos a la retención de los impuestos de ley.

| Tiempo          | Tasa   |
|-----------------|--------|
| 30 a 59 días    | 5,65%  |
| 60 a 89 días    | 5,90%  |
| 90 a 179 días   | 6,15%  |
| 180 a 269 días  | 6,65%  |
| 270 a 359 días  | 6,90%  |
| Más de 360 días | 7,90%  |
  
- [ ] Una base de datos que actualice toda la informacion de las instituciones financieras.

- [ ] Un back office con una vista de admin que permita editar y hacer mantenimiento de la informacion de instituciones financieras.

- [ ] Poner en produccion 


## Authors
- [Richard Palacios](https://richardpalaciosg.dev)
- [@rpalaciosg](https://github.com/rpalaciosg/)

## License

[MIT](https://choosealicense.com/licenses/mit/)


