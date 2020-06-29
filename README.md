# GeoSpartial-Data-Project

EL objetivo de este proyecto es encontrar la mejor localización para abrir una oficina de una empresa de diseño de juegos, y como data analytics nos piden que  según los siguientes requisitos demos unas coordenadas sobre el lugar exacto donde deseamos abrir nuestra oficina.

Estos son los requisitos sugeridos:

- Designers like to go to design talks and share knowledge. There must be some nearby companies that also do design.
- 30% of the company have at least 1 child.
- Developers like to be near successful tech startups that have raised at least 1 Million dollars.
- Executives like Starbucks A LOT. Ensure there's a starbucks not to far.
- Account managers need to travel a lot
- All people in the company have between 25 and 40 years, give them some place to go to party.
- The CEO is Vegan
- If you want to make the maintenance guy happy, a basketball stadium must be around 10 Km.
- The office dog "Pepe" needs a hairdresser every month. Ensure there's one not too far away.

El primer paso tomado ha sido analizar donde se situan en el mundo la mayor cantidad de empresas de gamers, este proceso se puede encontrar en el documento ``gettingtheplace.ipynb``. 
La conclusión obtenida fue que el mayor numero de empresas de gamers se encuentra en **San Francisco, CA** y filtramos más por zip_codes donde mayor número de empresas hay.

Una vez que tenemos filtrado por la ciudad de San Francisco, vamos a sacar usando las apis de **Google Places** , **Foursquare**  y **GeoCode** un listado de todos los requisitos previamente descritos, este proceso se puede encontrar en el documento `` Expectingrequirements.ipynb``.

Una vez sacado esta información creamos un mapa en TableauMap para ver todos los requisitos por layers. 
Este es el link al mapa:
https://public.tableau.com/profile/miriam6476#!/vizhome/officeHQ/SANFRANCISCOCA?publish=yes



Tras visualizar el mapa, voy a seleccionar las coordenadas de la empresa que más requisitos cumpla, esto lo realizo con **MongoDB** . Todo este analisis se puede encontrar en el documento ``Choosingthepoint.ipynb``

Finalmente esta son las coordenadas seleccionadas **37.780134,-122.396744** y se encuentra a esta distancia de los siguientes requisitos:

1. Club_distane : 0.4907764314669059 km
2. Court_distance: 1.7546611083781394 km
3. School:distance 0.9197809838870833 km
4. vegan_restaurant_distance 0.900747605269903 km
5. Offices_money_raised_over1M_distance :0.4453363851813138 km
6. airport_distance: 1.3210798150082281 km






