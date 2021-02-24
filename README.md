# worldtour-
try = ['US', 'Brasil', 'Peru']

US_city = ['NY', 'Chicago', 'LA']
NY_attraction = ['Empire State', 'Statute of Liberty']
Chicago_attraction = ['Willis Tower', 'Navy Pier']
LA_attraction = ['Disneyland', 'Hollywood']
US_city_attraction = {'NY': NY_attraction, 'Chicago': Chicago_attraction, 'LA': LA_attraction}

Brasil_city = ['Rio', 'Sao Paulo']
Rio_attraction = ['Cristo Redentor', 'Copacabana']
Sao_Paulo_attraction = ['Museu de Arte', 'Teatro Municipal']
Brasil_city_attraction = {'Rio': Rio_attraction, 'Sao Paulo': Sao_Paulo_attraction}

Peru_city = ['Lima', 'Cusco']
Lima_attraction = ['Plaza de Armas', 'Cathedral']
Cusco_attraction = ['Machu Picchu', 'Huamantay Lake']
Peru_city_attraction = {'Lima': Lima_attraction, 'Cusco': Cusco_attraction}

City_dict = {'US': US_city, 'Brasil': Brasil_city, 'Peru': Peru_city}

Attraction_dict = {'US': US_city_attraction, 'Brasil': Brasil_city_attraction, 'Peru': Peru_city_attraction}

city = input('would you like to see all the cities availble in our tour? (Y/N):    ')
while city == 'Y':
    print(US_city, Brasil_city, Peru_city)
    break
attraction = input('We have exciting attractions, would you like to see them all? (y/N)')
if attraction == 'Y':
    print('Attraction in our tour')
    for item in Attraction_dict:
        print(item)
