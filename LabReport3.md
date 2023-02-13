# Lab Report 3
## Charisse Chua 

The command line I decided to research more about was `grep`. These are the 4 commands: 
1. `grep -i`
2. `grep -w`
3. `grep -o`
4. `grep -v`
***
**1.** `grep -i`


`grep -i "PuertoRico" demoResults.txt` output:
```
written_2/travel_guides/berlitz2/PuertoRico-History.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
```

`grep -i "puertorico" demoResults.txt` output:
```
written_2/travel_guides/berlitz2/PuertoRico-History.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
```

`grep -i` ignores the case when searching for matching characters. This can be helpful because when you're searching for terms, you don't always know what the case is/don't need the case to match. In the second example, when I used just regular grep to search, it showed there were no files that matched that which can be misleading. 

**2.** `grep -w` 

`grep -r -w "some" written_2` vs `grep -r "some" written_2` output:

`grep -r -w "some" written_2` (shortened):
```
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:The small, flat island of Nueva Tabarca lies about an hour by boat from Alicante. (From mid-April to October, boats run daily from Alicante and Santa Pola, whence the sea voyage takes half as long. There is no service in the winter.) You won’t see any pirates here, as the last of them sailed away from their former stronghold in 1786. But you will find fishermen, many of whom are direct descendants of some 600 Genoese mercenaries King Charles III rescued from captivity on Tunisia’s Tabarka Island, hence the name. These people have made Nueva Tabarca their home for more than two centuries, in spite of poor fishing and the lack of doctor, priest, and schoolmaster. It was tourism that finally saved the declining population from fading away altogether, and provided islanders with a priest and teacher at last. Sun-seeking visitors, mostly Spaniards, flock to the island on Sundays, the most popular day for excursions. Even then, you’ll always be able to find peace and quiet on one of the tiny, seaweed-draped coves beyond the main sandy bay.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:From Jijona, continue along the N-340 to Alcoy, 56 km (36 miles) from Alicante. Don’t be disappointed by this grey industrial town, for it manufactures some of Spain’s most popular sweets: they are peladillas, Marcona almonds coated with sugar. Sometimes pine kernels are sugar-coated, too, and the delicious result is called pinyonets.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:From the town of Ibi onwards you’ll see many castles and forts, some of them visible for miles. They were strategically positioned by ever-vigilant Romans, Moors, and Christians.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:The Costa Blanca’s reputation for magnificent beaches and lively resorts comes from the northern stretch of coast. Take the N-332 from Alicante and drive through Campello to the fishing port of Villajoyosa. This picturesque village, some 30 km (18 miles) from the provincial capital, is more authentically Spanish in character than Benidorm, its cosmopolitan neighbour.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:La Vila, as Villajoyosa is affectionately called, boasts some Roman, Moorish, and Visigothic remains, and Spain’s oldest chocolate factories. But it’s the vivacious Moors and Christians fiesta, with its bare-bellied, flashing-eyed “slave-girls” and swashbuckling “corsairs,” that really makes the town unique. In the last week of July, many of the town’s 16,000 inhabitants parade and fight in richly costumed companies — los piratas, los tuareg, and los moros del Rif among them — re-enacting the defeat in 1538 of the Algerian pirate Zala Arráez, a Mediterranean scourge who started it all by sacking the castle in a daring dawn raid.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:Now make for Guadalest (some 10 km/6miles to the east), the Costa Blanca’s famed “eagle’s nest” fortress, built by the Moors 1,200 years ago. Inaccessible except for a tunnel carved through 15 metres (50 feet) of solid rock, Guadalest was never conquered, though James I of Aragon took it by siege during the 13th-century Reconquest. The fortress even withstood an earthquake in 1644, as well as attempts by the Austrian Archduke Charles to blast his way in during the War of the Spanish Succession. Guadalest itself is just as spectacular as the view from it. Wandering round the compact castle, you’ll understand why, for lack of space, the belfry had to be built outside, and why the picturesque old cemetery is so small.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:After Tárbena comes the finest scenery of all: bold, terraced mountains, wide undulating valleys, and scattered farms connected by mule tracks. In spring the countryside is covered with the pink and white of almond blossoms, but the road is for all seasons, with groves of gnarled olive trees alongside it, their leaves blowing silver in the evening light. Follow the road to Coll de Rates, 500 metres (1,500 feet) above the wide orange- and vine-filled plains that sweep up to Jávea, Denia, Gandía, and the deep-blue Mediterranean. Farther on, take the road to Jalon, where in late summer farmers sell muscat grapes to passers-by, and you can buy some of the strong local wine. Or carry on past Orba to Benidoleig and visit the prehistoric caves, Las Calaveras. Here high-domed ceilings drip with stalagtites, and human bones more than 50,000 years old have been found.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:The fishing port and resort of Santa Pola (18 km, south of Alicante on the N-332) has an extraordinary number of restaurants. Nearby waters, particularly rich in prawns and red mullet, provide all manner of eating houses, both on the beach and in the town, with some of the best seafood on the coast. There’s also a 14th-century castle and several good beaches with fine, white sand.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:The area of Mar Menor is also noted for its windmills, some of them restored to perfect working condition.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:Thousands upon thousands of date palms overwhelm the eye in Elche, a city as old as the Iberians. The trees, originally planted by the Carthaginians in 300 b.c. or thereabouts, thrive under irrigation. They still stand as the Moors described them, with “feet in water, heads in the fire of heaven.” Elche’s palms are watered by Abderraman III’s tenth-century irrigation system and surround the town of some 200,000 inhabitants on three sides.        
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:The Museo Municipal Mariano Benlliure, alongside the church, contains a collection of works in bronze, marble, and clay by the modern sculptor Mariano Benlliure (1868–1947), among them likenesses of the famous men of his day. You’ll also see some of his pasos — sculpture in life size or larger, a feature of religious processions, particularly during Holy Week.
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:Northwest of the city centre is the Ermita de Jesús church and its impressive Museo Salzillo. The highly important group of sculptures gathered here represents every facet of Francisco Salzillo’s work. During a career that spanned the 18th century, Salzillo produced large processional figures still carried in Holy Week celebrations, and small, intimate carvings, some of them on a miniature scale. Also with a visit is the Museo de Arqueologica, on the Calle Gran Via Alfonso, which traces the history of the region from Roman times.
written_2/travel_guides/berlitz2/Cuba-History.txt:In 1511 Diego de Velázquez sailed from neighboring Hispaniola with some 300 conquistadores (conquerors). Baracoa became the first of seven settlements across Cuba. Velázquez and his followers enslaved the native peoples and in the process exposed them to European diseases. Whole villages committed suicide, and by the mid-1500s the Indian population had declined from over 100,000 to 3,000.
written_2/travel_guides/berlitz2/Cuba-History.txt:Spaniards born and raised in Cuba, known as criollos (creoles), managed the sugar-cane plantations but were not involved in the running of the country. During the 19th century some criollos (particularly in Oriente, the island’s poorer, eastern region) became increasingly disenchanted and desired greater autonomy.
written_2/travel_guides/berlitz2/Cuba-History.txt:In 1895 José Martí, Cuba’s most venerated patriot (who now has a street, square, or building named after him in every town), led the next and most important uprising against Spain. Born in 1853 and exiled at 18 for his political views, Martí became a journalist and poet. From exile in the United States he argued for Cuban independence. Martí was killed in an ambush during the War of Independence, which began in 1895 and in which some 300,000 Cubans died.
written_2/travel_guides/berlitz2/Cuba-History.txt:For the next five decades the United States, the largest importer of Cuban sugar, dominated the island’s economy and largely controlled its political processes. The period was rife with political corruption, violence, and terrorism. After 1933 Fulgencio Batista, though only a sergeant, orchestrated the strings of power through a series of puppet presidents before winning the presidency outright in 1940. He retired in 1944 but returned by staging a military coup in 1952. His venal dictatorship made it possible for him to invest some $300 million abroad by 1959.
written_2/travel_guides/berlitz2/Cuba-History.txt:Washington remained fundamentally opposed to Cuba’s political evolution and sought to isolate Castro in Latin America. Soon after the Bay of Pigs, Castro declared himself a Marxist-Leninist. Castro had not displayed any Communist inclinations in the 1950s, and some suggest that US aggression pushed him to ingratiate himself with the powerful Soviet Union and its Eastern block of potential trading partners. By the end of the 1980s, more than 80 percent of Cuban trade was with the USSR, which also provided Cuba with a subsidy of state support worth an estimated US$5 billion annually.
written_2/travel_guides/berlitz2/Cuba-History.txt:The dangers of exposure to foreign opinion and “moral corruption” from the rapidly expanding tourism industry is now viewed as a necessary evil. The adoption of measures such as the legalization of the dollar and small-scale private enterprises in 1993, and the introduction of private farmers’ markets in 1994, have improved the welfare of some Cubans. The situation for others, with no access to dollars, has turned increasingly desperate.
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:Cubans crave live music, and — with the surge in international popularity of traditional Cuban music — so do most visitors to Cuba. You certainly won’t have to go out of your way to hear music performances. Roving groups of musicians can be found playing everywhere from airports to restaurants. Merely wandering the streets of Havana, Santiago, or Trinidad, you’re likely to stumble across a party with a live band, or even a back alley where some impromptu jamming is going on. On Saturday nights in Camagüey, the music spreads to the streets in a “Noche Camagüeya” block party along Calle República.
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:The Tropicana in Havana (Calles 72 and 43, Marianao; Tel. 33-7507), founded in 1939 in a dazzling open-air arena, is indisputably the queen of cabarets. The likes of Nat King Cole performed here in pre-revolutionary times. With a 32-piece orchestra and a cast of over 200 (some parading in impossibly large headdresses), the sheer scale of the spectacle will make your head spin. The show regularly kicks off at 9:30pm, and a shorter performance follows later; there are also a restaurant and disco. Reservations and transportation can be arranged at your hotel for US$60. You can always visit independently, but the venue, situated in the suburb of Marianao, is tricky to find, and you might arrive only to find no tickets remaining. Havana’s next-best cabaret show, smaller and less expensive, is Cabaret Parisien, at the Hotel Nacional (Calles 21 and O, Vedado; Tel. 30-3564), nightly at 10:30pm; admission is US$35.
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:In Varadero, the Cabaret Continental at the Hotel Internacional (shows nightly from 8:30pm to 3am) pales in comparison with the former venues but is nonetheless an enjoyable and sometimes fairly raunchy song-and-dance extravaganza. A fun show — kind of Afro-Cuban with a pirate theme — followed by disco takes place in a cave at the Cueva del Pirata, some 9 km (6 miles) east of Varadero (Autopista Sur, km 11), nightly at 10:30pm until the wee hours. There is also a cabaret at the Meliá Varadero hotel.
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:Both bars and cafés are places to have a mojito, daiquiri, or shot of ron (rum), smoke a Cohiba, and — usually — hear some live Cuban rhythms. In Havana the bars not to miss are Hemingway haunts: La Bodeguita del Medio and El Floridita. Enjoyable café-bars in Havana include Café de Paris (Obispo and San Ignacio), Café O’Reilly (O’Reilly and San Ignacio), Montserrate (Avenida de Bélgica and Obrapía), and El Patio (Plaza de la Catedral). Several hotels also have good bars, including Hotel Sevilla (made famous in Graham Greene’s Our Man in Havana), Hotel Inglaterra’s rooftop bar, and Hotel Havana Libre’s Turquino (with amazing views from the 25th floor).
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:To the surprise of many first-time visitors, Cuba is no speck in the Caribbean. Nicolás Guillén, the nation’s finest poet, described the island as a “long green alligator.” Long it certainly is, at 1,250 km (776 miles) from snout to tail. Nearly the size of England, Cuba is divided into 14 provinces and incorporates some 1,500 offshore islands, known as cayos (“cays” or “keys”).
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:Given its size, you would need at least a month to explore Cuba fully. Most people begin their journeys in the capital, Havana, before heading to the prized tobacco lands farther west and doubling back across the plains of sugar cane and some of the country’s finest colonial towns in central Cuba. The eastern region, known as Oriente, has soaring mountains and Cuba’s second and most musical city, Santiago de Cuba.
```

`grep -r "some" written_2` (shortened):
```
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:City Tours of both Puerto Vallarta and Manzanillo are offered by virtually every local tour operator. Bay Tours are very popular in every coastal destination from Puerto Vallarta down to Huatulco, and are also an excellent way to get your bearings, from the vantage point of the waters offshore. In Puerto Vallarta, a cruise may be on any type vessel, from a charter sailboat to an oversize catamaran, even to an exact replica of Christopher Columbus’s Santa Maria. There is something to fit every taste. Both day and sunset cruises are offered; day cruises generally include visits to funky or secluded beaches that are only accessible by boat. In Acapulco the Yate Fiesta and the Aca Tiki are the long-running favorites for sunset cocktail cruises..
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:Another specialty of Acapulco are the glass-bottom boat tours to La Roqueta, where for US$4 you can view something unique and characteristic of Mexico’s spirit — an underwater statue of the Virgen de Guadalupe. In Zihuatanejo, an elegant trimaran glides along the small bay for a memorable sunset cruise. In Huatulco a tour of the nine bays is a considered a “must” to truly experience the place; you can hire a panga from the well-organized fisherman’s cooperative or join one of the organized tours offered by several local tour operators. Both depart from the marina in Santa Cruz.
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:Mexico is a country that welcomes children. You will find very few places that do not include some kind of family-oriented attraction. Puerto Vallarta, with its miles of beaches, is among the most appropriate resorts for families. Most four- and five-star hotels offer supervised “Kids Clubs” and organized children’s activities for a nominal daily fee.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:The cultural scene has blossomed as well, with Vallarta — as it is called by the locals — now considered among the country’s leading art centers. Especially during the winter months, an almost constant succession of gallery openings and exhibitions attracts creative talent from throughout the Americas. The culinary community has taken numerous awards and accolades back to this seaside town, where more than 250 restaurants offer gourmands their own piece of paradise. Yet what makes this place overwhelmingly attractive is its total lack of pretense and completely comfortable ambiance — it remains down-to-earth, genuinely casual, and simply irresistible.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:Though some travelers have expressed concern that Vallarta has grown too much in recent years, the town’s geography has imposed clear boundaries, allowing development to gradually expand to the north and south of the central downtown area. Within the town itself, the city government has strict guidelines that ensure the architectural integrity of Vallarta, and in recent years has implemented a successful campaign to maintain the cleanliness of the town.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:South of El Centro, yet still considered to be a part of Viejo Vallarta, is the area alternately known as “Los Muertos” and “Zona Romántica.” The neighborhood is named for the main beach in town, Los Muertos (the Dead) — however, the city fathers prefer a kinder, gentler nomenclature, and have unsuccessfully tried to rename it “Zona Romántica,” and the beach, “Playa del Sol” (just so you’ll know when you see the many street signs). From family-run beachfront hotels to eclectic inns poised on the surrounding hills, here is where you feel the essence of Vallarta’s charms — the area preferred by independent travelers and repeat visitors. New sidewalk cafés, bookstores, and martini bars have popped up along the main road, Olas Altas, giving it a decidedly bohemian, funky feel. This part of town also is home to “Restaurant Row” (along Basilio Badillo) and Rockin’ Row (Ignacio L. Vallarta, just beyond the southbound bridge). This perpendicular meeting of streets contains something for every taste and budget, in both dining and nightlife.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:About seven miles west of downtown, lies the Península de Santiago, Manzanillo’s best known landmark. For many travelers, this town is synonymous with the famed all-white world of Las Hadas (“the Fairies”) and its adjoining golf course. Set on a southern promontory of Santiago Peninsula, Las Hadas gazes across Manzanillo Bay to the town, but is a world apart in character. Its Moorish architecture, which looks something like a setting for Arabian Nights, became renown as the place where Bo Derek showed her appreciation for Ravel’s bolero in the movie Ten. Las Hadas was built in the 1970s by the Bolivian tin multimillionaire Antinor Patiño as a private, super-exclusive resort and a respite from Acapulco’s excessive glitz. Its presence spawned construction up and down the adjoining beaches, making Santiago Peninsula the most desirable address in town, especially for visitors to Manzanillo.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:Playa Las Gatas, once a walled pre-Hispanic wading pool, earned its name from the whiskered nurse sharks that used to frequent the surrounding wall. Today Las Gatas is the most pleasant beach for swimming and children’s activities. The coral beach has exceptionally clear waters, with little or no surf, and practically no undertow. Located across the bay from Playa La Ropa, it is easily reached by a short ride aboard small, shaded boats that run from the Muelle (the town pier) every 10-minutes. Open air restaurants, some fancier than others, offer local delicacies, including extraordinarily fresh pink-tongued clams. Las Gatas is a departing point for dive trips to some excellent sites.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:The first beach in Ixtapa, coming from Zihua is Playa Hermosa, which can only be accessed through the Westin Hotel. This small beach is dramatically framed by rock formations. The surf varies seasonally from minimal to quite rough, and has become somewhat of a private beach for Westin’s guests.
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:As it fell out of favor as an international darling, its prices adjusted out of necessity. Now, some exceptional values in hotels and dining can be found, and today Acapulco is considered a value-packed destination, attracting more Mexican national than foreign tourism.
```

`grep -r -w "something" written_2` output (shortened):
```
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt:Clothing. You are sure to find something that fits your personal taste in summer attire in the Yucatán. Designer labels from the US and Europe are abundant in the tourist-zone malls in Cancún. Smaller stores throughout the region are filled with attractive beachwear, T-shirts, hats, footwear, and cool, comfortable cotton dresses, skirts, and sarongs that are ideal for the warm climate here.
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:You can sunbathe on the beach at the site; some Mexican families spend the day here, something the Maya would never have been able to do when it was a religious center. Only those who belonged to the upper and religious castes were allowed into its inner sanctum.
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:Uxmal was a very rich city at the height of its powers and protector of many smaller settlements, which paid tribute to it both in food and money. A string of these sites now forms what is called the Puuc Route, and they can all be visited in one day. Though small, each one has something different to reveal.
written_2/travel_guides/berlitz2/China-WhatToDo.txt:Since the distribution system is unpredictable, old China hands say you shouldn’t take a chance: if you find something you like, buy it, for it might not be on sale anywhere else. Prices are as marked; do not try to bargain.
written_2/travel_guides/berlitz2/China-WhereToGo.txt:In the Middle Ages, the emperors decided to do something about the capital’s unrelieved flatness. They ordered hills to be artificially constructed just north of the Forbidden City so they could go up and, in total privacy, enjoy a summer breeze and a bird’s-eye view over the curved tile roofs of their imperial compound. Try it yourself, perhaps at dawn, when a thin haze drapes itself over the pavilions, redefining yet softening the features of this storybook skyline. You’ll see why the emperors wanted it all for themselves.
written_2/travel_guides/berlitz2/China-WhereToGo.txt:Balmy and often misty weather keeps Chengdu green and full of flowers year ‘round. It’s the climate in which bamboo thrives, and bamboo is the staple of the giant panda. The best place to spot these cuddly-looking beasts in something resembling the wilds is at the China Research Base of Giant Panda Breeding, 11 km (7 miles) northeast of downtown Chengdu, where a dozen pandas have free run of some 30 hectares (80 acres) of bamboo groves. There’s a panda museum here, too. In closer confines, the Chengdu Zoo has more resident pandas (about a dozen) than does any other zoo in the world. The thin bamboo stalks they find so delicious are grown right in the grounds. Because they are the stars of this attraction, the giant pandas are assigned high-ceilinged, spacious cages and outdoor play areas.
```

When just using the regular `grep -r "some"` to recursively search for the word through all the files in written_2, it displays all of the words that have "some" in it, even if it's a substring. The output was difficult to document, but from the screenshot you can see that both "sometimes" and "something" were included. If I wanted to just search for the word "some" and no other words where "some" is a substring, then it is helpful to use `grep -w`. It will search for only when that word stands alone, not when it's part of another word.


**3.** `grep -o` 


`grep -r -o "nowhere" written_2` output:
```
written_2/non-fiction/OUP/Fletcher/ch2.txt:nowhere
written_2/non-fiction/OUP/Fletcher/ch5.txt:nowhere
written_2/non-fiction/OUP/Fletcher/ch9.txt:nowhere
written_2/non-fiction/OUP/Fletcher/ch9.txt:nowhere
written_2/non-fiction/OUP/Kauffman/ch3.txt:nowhere
written_2/non-fiction/OUP/Kauffman/ch6.txt:nowhere
written_2/non-fiction/OUP/Kauffman/ch6.txt:nowhere
written_2/travel_guides/berlitz1/HistoryHawaii.txt:nowhere
written_2/travel_guides/berlitz1/IntroJapan.txt:nowhere
written_2/travel_guides/berlitz1/IntroJapan.txt:nowhere
written_2/travel_guides/berlitz1/WhatToIbiza.txt:nowhere
written_2/travel_guides/berlitz1/WhatToMadeira.txt:nowhere
written_2/travel_guides/berlitz1/WhereToHongKong.txt:nowhere
written_2/travel_guides/berlitz1/WhereToIbiza.txt:nowhere
written_2/travel_guides/berlitz1/WhereToIbiza.txt:nowhere
written_2/travel_guides/berlitz1/WhereToIndia.txt:nowhere
written_2/travel_guides/berlitz1/WhereToItaly.txt:nowhere
written_2/travel_guides/berlitz1/WhereToItaly.txt:nowhere
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:nowhere
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:nowhere
written_2/travel_guides/berlitz2/China-WhereToGo.txt:nowhere
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:nowhere
written_2/travel_guides/berlitz2/NewOrleans-History.txt:nowhere
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:nowhere
```

`grep -r "nowhere" written_2` output (shortened):
```
written_2/travel_guides/berlitz1/HistoryHawaii.txt:        The war broke out in Hawaii as nowhere else in America with
written_2/travel_guides/berlitz1/IntroJapan.txt:        metal balls going nowhere. Back home, wives who at first seem passive  
written_2/travel_guides/berlitz1/IntroJapan.txt:        rewarded by unexpected and unforgettable experiences available nowhere 
written_2/travel_guides/berlitz1/WhatToIbiza.txt:        •The truly local art form, found nowhere else, is Ibicenco
written_2/travel_guides/berlitz1/WhatToMadeira.txt:        nowhere are they so accessible and do they cover such great area. The
written_2/travel_guides/berlitz1/WhereToHongKong.txt:        nowhere, Hakka women in their traditional flat straw hats with hanging
written_2/travel_guides/berlitz1/WhereToIbiza.txt:        lively  — offers things seen nowhere else on earth. Whether your     
written_2/travel_guides/berlitz1/WhereToIbiza.txt:        which just seems to rise from nowhere out of the ocean.
written_2/travel_guides/berlitz1/WhereToIndia.txt:        these bizarre shapes, staircases going nowhere, and windows in walls 
written_2/travel_guides/berlitz1/WhereToItaly.txt:        gondola that appears out of nowhere. Staying forever is most likely to
written_2/travel_guides/berlitz1/WhereToItaly.txt:        Probably nowhere is there so much spectacular painting on
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:Fortuna utca is a charming, much-photographed street full of pastel-painted houses and takes its name from a tavern which stood at number 4 from 1785 to 1868. Today this houses the Museum of Commerce and Catering (Kereskedelmi és Vendéglátóipari Múzeum) — nowhere near as grand (nor as boring) as its name suggests — dealing with confectionery in one section and Hungarian trade in the late 19th and early 20th century in another. The museum curators take a genuine delight in demonstrating various exhibits: it’s well worth a visit.
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:La Gomera is, indeed, a dramatic and rugged mountainous island. It has a coastline that is dominated by dramatic cliffs — there are very few beaches, and the interior is full of vertiginous, mostly verdant, valleys that are often lined with narrow fields stepped into the sides of the mountains. For extra effect these valleys are more often than not covered by a ceiling of cloud, whisked in by the trade winds, which seem to perpetually hang over the island. In the center, there is the unusually dense growth of trees and fauna in what is the Parque Nacional Garajonay (open Tuesday–Sunday 9:30am–4:30pm). Less than 20 km (121⁄2 miles) from north to south, this amazing island has been declared a Property of Humanity by UNESCO. In fact, a third of the island, 12,450 hectares (30,774 acres) has been designated into seventeen protected areas. Such terrain, though, makes for difficulty in getting around, and even the Romans, had they ventured this way, would have found their legendary ability to build straight roads put to an impossible test. In fact, almost nowhere on the island will you find a straight stretch of road, everywhere you go the roads twist and turn continually, often turning back on themselves in hairpin bends. Making driving even more complicated is the fact that the roads, although improving, are often of poor quality, and the directional signs leave much to be desired.
written_2/travel_guides/berlitz2/China-WhereToGo.txt:Xi’an has two fine museums. The Shaanxi Provincial Museum (Shaanxi Shengbowuguan), occupying the 14th-century grounds of the Temple to Confucius, holds a rich store of art works and rare artifacts: funerary figurines, traditional paintings, ancient household equipment, and huge bronzes masterfully cast 3,000 years ago. But the chief focus must be on the museum’s famous Forest of Steles (Beilin). This library of inscribed stone slabs, including a complete edition of the Confucian classics (carved in a.d. 837), documents the history of Chinese culture and calligraphy. The Nestorian Stele records another history altogether, that of Christianity in China from 635 to 781. The art of calligraphy is exalted in this museum as nowhere else. The street leading to the old museum along the southern city wall, Shuyuanmen, has been restored and offers a fine collection of traditional art and calligraphy shops.
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:sun, sand, and sangría. Since then, it has built, quite literally, on that reputation. And although it is nowhere as inexpensive, even relatively, as it once was, it is still a highly popular tourist destination.
written_2/travel_guides/berlitz2/NewOrleans-History.txt:Law brokered a deal with the French government, giving him a 25-year charter to develop the Louisiana Territory. All he needed were investors and settlers, whom he lured with a campaign of propaganda. On posters Law distributed in France, New Orleans was pictured as a prosperous seaport. When Law’s clients arrived after months at sea, the truth of the Mississippi Bubble was plain. The only housing available was huts or tents, and the roads were generally quagmires. But there was nowhere else to go, so the pioneers were forced to pitch in and try to survive.
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:Another majestic view of the city is from a charming park, Miradouro de Santa Luzia, just down the hill from the castle. Lisbon’s Sé Patriarcal (cathedral) appears out of nowhere at a bend in the road (most easily reached from the center by continuing east on the extension of Rua da Conceição). Begun as a fortress-church in the 12th century, its towers and walls suggest a beleaguered citadel. Adjacent to the cathedral is the lovely Igreja de Santo António da Sé, named for Lisbon’s patron saint, St. Anthony of Padua.
```
In the first example, when I use `grep -o` it shows just the file names and the matching word. It doesn't display all the lines before/after it. This can be helpful when you just want to see the matching word directly next to the file name. It makes it much cleaner and less data to sort through. If you look at the second example where there is no `grep -o`, it displays all the surrounding lines around the word you're searching for, which is difficult to analyze and not always necessary. 

**4.** `grep -v`

`grep -v "txt" demoResults.txt` output: 
```
written_2/
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Rybczynski
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```

`grep -v "travel-guides" demoResults.txt` output: 
```
written_2/
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chO.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Rybczynski
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/demoResults.txt
```


`grep -v` searches for lines that don't match the given pattern/string. In the first example, it prints only the file names that don't have "txt". This can be helpful if you are searching through files and don't want a certain type of file to be returned, such as ".txt" or ".java". The second example returns only the file names that aren't in "travel-guides." This can also be helpful if you want to sort through different directories so that you can sort out what you don't want to have.

Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/
