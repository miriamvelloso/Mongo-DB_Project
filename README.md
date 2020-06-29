# GeoSpartial-Data-Project

EL objetivo de este proyecto es buscar las coordenadas ideales para abrir una oficina según los siguientes requisitos:

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

Una vez que tenemos filtrado por la ciudad de San Francisco, vamos a sacar usando las apis de **Google Places** y **Foursquare** un listado de todos los requisitos previamente descritos, este proceso se puede encontrar en el documento `` expectingrequirements.ipynb``.

Una vez sacado esta información creamos un mapa en Tableau Public para ver todos los requisitos por layers. 
Este es el link al mapa:
https://public.tableau.com/profile/miriam6476#!/vizhome/officeHQ/SANFRANCISCOCA?publish=yes




