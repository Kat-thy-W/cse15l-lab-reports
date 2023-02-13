# Less Command Options in Linux
 The less command shows a file (or files) contents one screen at a time, use q to quit the pager mode.

## Display Line Number with Less
less - N \
source: https://linuxhandbook.com/less-command/
### example 1:
We use less to access the content of a file, and the -N option show the line number of the content of the txt file, which give use and idea of how the content was organized.
```
input: 
$ less -N written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
  
output:
      1
      2
      3
      4
      5 What To Do
      6 Spend any time in this area, and you’ll quickly realize that life along Pacific Mexico is much more than “just a beach.” There is a wealth of outdoor adventures, cultural encounters, and the simple pl      6 easures of local village life .
      7 Entertainment
      8 Fiestas
      9 Mexico is known for its countless festivities and perennial spirit of celebration — Mexicans may have even invented the “art of the party.” In Mexico, it’s a given that any reason is a reason to celeb      9 rate, and traditional fiestas will include the entire family, with plenty of food and drink, contributed by all those involved.
     10 Mexico’s folkloric traditions have become the centerpiece of the modern “Mexican Fiesta,” created especially with the tourist in mind. These full evenings of entertainment generally include a makeshif     10 t marketplace featuring artesanía for sale, a buffet Mexican dinner, games (involving drinking large quantities of tequila), mariachi music, a presentation of folkloric dance from around the country,      10 and a generous supply of margaritas and other beverages. Most of the time these are smallish presentations, with dances performed by amateur groups; at their worst, they can be truly gaudy and almost      10 laughable shows.
     11 The exception is in Acapulco. The Centro de Convenciones offers arguably the best Fiesta Mexicana in the country, and is the closest you’ll come to an authentic display of Mexican culture and dance. A     11 long with beautifully performed folkloric dances from all over Mexico, you’ll witness a pre-Hispanic ceremony called Los Voladores de Papantla, which represents an invocation to the four cardinal poin     11 ts and a prayer for fertility; a floreador roping exhibition; and the vibrant sounds of the mariachi. This fiesta is held every Monday, Wednesday, and Friday from 7 to 10pm. Reservations are recommend     11 ed, to ensure a good table. For reservations, call Tel. (7) 484-7046.
     12 In Puerto Vallarta one fiesta that stands out from the rest is not a traditional Fiesta Mexicana at all, but an evening at the secluded Caletas cove, accessible only by boat. Ritmos de la Noche (“Rhyt     12 hms of the Night”) is a truly magical experience. You travel by fast catamarans to the former home of John Huston, where you’ll be greeted by native drums and abundant tiki torches — there is no elect     12 ricity here — then dine by candlelight at tables set along the secluded beach. Following dinner, the jungle, sounds of nature, and a replica of a pyramid are the backdrop for a performance of pre-Hisp     12 anic dances with a unique contemporary choreographic twist. The show is held from Monday through Saturday. Call Tel. (3) 221-0657, for reservations.
     13 Nightlife
     14 Any place built on pleasing vacationers is bound to have its share of nocturnal attractions. Along Pacific Mexico, the options are as varied as the towns themselves, ranging from the dazzling discos o     14 f Acapulco to the quaint weekly “dances” on dirt floors in Barra de Navidad.
     15 Puerto Vallarta is making a name for itself with its vast selection of live music. One stretch of street — Ignacio L. Vallarta, just across the southbound bridge — is known as Rockin’ Row, for its ecl     15 ectic collection of clubs. Within easy walking distance from one another, you’ll find a blues club, a Harley-Davidson-theme rock n’ roll club, a salsa dance club, live mariachi music, a glitzy gay clu     15 b (with nightly leather ranch-hands’ show), an alternative dance club, and a sports bar.
     16 Still, the malecón rules when it comes to sheer rowdy nighttime fun. Along with the longstanding Carlos O’Brians, several open-air bars and dance clubs stay open until 5am, and a new Cuban restaurant-     16 bar pleases patrons with authentic food and live music nightly until 3am. Just a few blocks in back of the malecón are a growing collection of unique clubs with a more urban edge. Among them is La Can     16 tina, a hipper version of a Mexican classic. By day it serves classic cantina fare, by night it clamors with the sound of conversation mixed with the best in contemporary recorded Mexican music. Board     16  games are available for play.
     17 Marina Vallarta is quieter at night, with the lighthouse-top lounge, El Faro, a favorite for spending a romantic evening, listening to live flamenco guitar. Along the Hotel Zone, the throwback disco C     17 hristine still manages to draw a crowd for the nightly midnight laser show, and J&B is a very hot spot for true Latin dancing; a favorite with locals, it’s open until 5am. Also downtown, you’ll find t     17 he imported Hard Rock Café, Planet Hollywood, and Hooters, but they tend to draw lesser crowds than the locally-owned options.
     18 You’ll find a more traditional nightlife, consisting of a weekly “dance” that takes place in an outdoor stadium or on a makeshift dance floor in smaller coastal towns such as Yelapa, Cruz de Loreto, a     18 nd Barra de Navidad. Banda or ranchero-style music tends to dominate, but anything from hip-hop to classic rock may be tossed in for good measure.
     19 Manzanillo, Ixtapa, and Zihuatanejo offer less in the way of nightlife. Manzanillo’s clubs are few, but crowded, and feature recorded music for dancing. The Latin music clubs get going around 10pm, an     19 d don’t even show up before midnight at the techno and alternative clubs. The majority of clubs, and the ubiquitous Carlos ‘n’ Charlie’s, are located along the main boulevard, Miguel de la Madrid. In      19 Ixtapa, sunset happy hours offer the most options, and Mexican fiestas seem to be a “best bet” for a complete evening. Other later night offerings are a sampling of what you’ll find in any resort town     19  in Mexico: Christine’s disco at the Krystal Hotel, Sr. Frogs, and Carlos ‘n’ Charlie’s. The only really original option here is the club, La Valentina, a combination restaurant/video bar with a deser     19 t-inspired décor.
     20 There is no doubt that Acapulco rules when it comes to nightlife. In fact, I would venture that most visitors here come especially for that. Anyone that believes disco is dead hasn’t been to Acapulco      20 — it’s alive and well, and happens nightly in an array of clubs that get going around midnight and often close after the sun comes up. The most majestic of these, Enigma, Palladium, and Fantasy, are lwritten_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
```
### example 2:
use less -n to access content of two files at the same time. During the viewer mode, use :n (view next) and :p (view previous) to navigate between two files
```
input:
$ less -N written_2/travel_guides/berlitz1/HandRHawaii.txt written_2/non-fiction/OUP/Kauffman/ch4.txt

output:
(first file)
      1
      2
      3
      4
      5
      6         Oahu (Including Honolulu)
      7         Aston Waikiki Sunset $$$ 229 Paoakalani Avenue, Honolulu, HI
      8         96815; Tel. (808) 922-2700 or (800) 336-5599; fax (808) 922-8785;
      9         <www.aston-hotels.com>. One of Aston’s many condominium resort
     10         properties, this modern high-rise has large rooms with complete
     11         kitchens. Lanais afford views of the Diamond Head end of Waikiki Beach.
     12         410 rooms.
     13         Halekulani $$$$ 2199 Kalia Road, Honolulu, HI 96815; Tel.
     14         (808) 923-2311 or (800) 367-2343; fax (808) 926-8004;
     15         <www.halekulani.com>. Very large rooms, most facing the ocean,
     16         and luxurious bathrooms with robes, make this a “House Befitting
     17         Heaven,” the meaning of its Hawaiian name. With plenty of beachfront, a
     18         top French restaurant (La Mer), and the serene House Without A Key
     19         outdoor lounge for sunset drinks, Halekulani is a complete resort. 454
     20         rooms.
     21         Hilton Hawaiian Village $$$–$$$$ 2005 Kalia Road, Honolulu,
     22         HI 96815; Tel. (808) 949-4321 or (800) 445-8667; fax (808) 947-7898;
     23         <www.hawaiianvillage.hilton.com>. Waikiki’s larg­est resort
     24         covers 22 beachfront acres of gardens, lagoons, waterfalls, coconut
     25         palms, and swimming pools. There are dozens of shops, a spa, and a
     26         branch of the Bishop Museum in the Kalia Tower. Families love this
     27         city-within-a-city on the beach. 2,998 rooms.
     28         Hyatt Regency Waikiki $$$–$$$$ 2424 Kalakaua Avenue,
     29         Honolulu, HI 96815; Tel. (808) 923-1234 or (800) 233-1234; fax (808)
     30         923-7839; <www.hyattwaikiki.com>. The Hyatt’s two
     31         recently-renovated 40-story towers cover a city block at the Diamond
     32         Head end of Waikiki’s shopping avenue (across the street from the
     33         beach). 1,241 rooms.
     34         Ihilani Resort & Spa $$$$ Ka Olina Resort & Marina,
     35         92-1001Olani Street. Kapolei, HI 96707; Tel. (808) 679-0079 or (800)
     36         626-4446; fax (808) 679-0080; <www.ihilani.com>. A luxury resort
     37         on the west side of Oahu, expertly managed by JW Marriott, Ihilani is
     38         situated within a 640-acre resort community that provides golf, tennis,
     39         3 miles of beaches and lagoons, and a world-class spa within a
     40         half-hour drive of Honolulu. 387 rooms.
     41         Kahala Mandarin Oriental Hawaii $$$$ 5000 Kahala Avenue,
     42         Honolulu, HI 96816; Tel. (808) 739-8888 or (800) 367-2525; fax (808)
     43         739-8800; <www.mandarin-oriental.com/­kahala>. Graceful, elegant,
     44         and refurbished for the new century, the venerable Kahala artfully
     45         mixes Hawaiian, Asian, and international touches. There’s a private
(second file)
      1
      2
      3
      4
      5 Chapter 4
      6 Propagating Organization
      7 his book, with its curious title, Investigations, seeks new questions about the universe. It is not always that everything is hidden and science must ferret out the mysteries by scouring for unknown f      7 acts, although often science proceeds in the manner of finding new facts. Rather it can be the case that the world is bluntly in front of us, but we lack the questions of the world that would allow us
      7  to see. There are stories, perhaps merely stories, of the response to early Spanish ships in the Caribbean by native inhabitants. The ships were not seen  there was no concept for them.
      8 Bluntly in front of us: The closure of catalytic and work tasks in an autonomous agent by which it genuinely constructs a rough second copy from small building blocks by adroit linking of exergonic an
      8 d endergonic processes. A cell, or colony of cells, is propagating this organization of process.
      9 My aim in the current chapter is to begin to investigate what we might mean, and hence see, by propagating organization. No easy journey, this. I will begin with Maxwell’s demon and why measurement of      9  a system only pays in a nonequilibrium setting. In a nonequilibrium setting, the measurements can be stored and used to extract work from the measured system. Maxwell’s demon is the clearest place in      9  physics where matter, energy, and information come together. Yet, we will find the demon and his eorts at measurement tantalizingly incomplete: You see, only some features of a nonequilibrium system,      9  if measured, reveal displacements from equilibrium from which work can, in principle, be extracted. Other features, even if measured, are useless for detecting such energy sources from which work can      9  be extracted. Thus, whatever the demon’s eorts, there remain the issues of just what features of a nonequilibrium system the demon must measure such that work can be extracted, how the demon knows to      9  measure those features rather than other useless features, and how, once measured, couplings come into existence in the universe that actually extract work. Not good enough, I shall say, to assert th
      9 at in principle, work can be extracted. How does work come to be extracted?
     10 A simple example of a device that detects displacements from equilibrium and extracts work is a windmill. The vane on the windmill in eect measures the direction of the wind and pivots the windmill su     10 ch that its fan blades are perpendicular to the wind. In turn, the wind does work on the blades, causing the windmill to rotate. The system as a whole measures a deviation from equilibrium (here, the 
     10 direction of the wind), orients the entire system such that extraction of work by the wind is possible for the device, and it actually extracts work. The windmill turns.
     11 The universe as a whole  from galaxies to planetary systems, and certainly our and any other biospheres  is filled with entities that measure displacements from equilibrium that are sources of energy,     11  those entities actually do extract work. Think of the teeming busyness of a coevolving mixed microbial community of long ago, successfully linking exergonic and endergonic reactions fired by the sun      11 and other high-energy sources. That community measured displacements from equilibrium, extracted work, and inhabited Manhattan three billion years ago, literally building high-rise microbial mat ecosy
     11 stems. Its microbial descendants are constructing similar high-rise structures in the Sea of Cortez and on the Great Barrier Reef of Australia today.
     12 Where did all this come from, this measuring of useful displacements from equilibrium from which work can be extracted, the devices coupling to such measurements, and the extraction of work used to bu     12 ild up new kinds of devices that measure new kinds of displacements from equilibrium to extract work in new ways? Yet a biosphere, actually constructing itself up from sunlight, water, and a small div     12 ersity of chemical compounds, does all this over evolutionary time. The biosphere does achieve persistent measuring of displacements from equilibrium from which work can be extracted and does discover
     12  “devices” to couple to those energy sources such that work can be extracted.
     13 And since the biosphere does this, and the biosphere is part of the universe, then the universe does it. This coming into existence of self-constructing ecosystems must, somehow, be physics. Thus, it      13 is important that we have no theories for these issues in current physics. The stark fact that a biosphere builds up this astounding complexity and diversity suggests that our current physics is missi     13 ng something fundamental. A biosphere becomes complex, the universe becomes complex. I will argue that the very diversity and complexity of a biosphere begets its further diversification and complexif
     13 ication. I strongly suspect that the same is true of the universe as a whole. The universe’s very diversity and complexity begets its further diversification and complexification.
     14 After exploring Maxwell’s demon, I will ask a physicist’s question, What is work? Physicists have an answer  work is force acting through distance  given by a single number, or scalar, representing th     14 e sum of the force acting through the distance. But it will turn out that in any specific case of work, the specific process is organized in some specific way. Work is more than force acting through d
     14 istance; it is, in fact, the constrained release of energy, the release of energy into a small number of degrees of freedom. It is the constraints themselves  with, as Phil Anderson points out, a kind     14  of rigidity  that largely constitute the organization of the process. But  and here will be the hook  in many cases it takes work to construct the constraints themselves. So we will come to a terribl
     14 y important circle, work is the constrained release of energy, but it often takes work to construct the constraints.
     15 A conceptual cluster lies at the heart of the mystery. The cluster concerns the progressive emergence of organization in the evolution of the physical universe and of a biosphere. That emerging organi     15 zation concerns the appearance in the evolving universe of entities measuring relevant rather than nonrelevant properties of nonequilibrium systems, by which they identify sources of energy that can p     15 erform work. Then physical entities appear that construct constraints on and couplings to the release of the identified source of energy whereby the energy is actually released and work comes to be pe     15 rformed. Such work often comes to be used to construct further detectors of energy sources and entities that harbor constraints on the release of energy, which when released constitutes work that cons     15 tructs still further sources of energy and constraints on its release. It should be clear that we have at present no theories about these matters, nor even a clear concept of the subject matter of suc
     15 h theories.
     16 The heart of the mystery concerns a proper understanding of “organization” and “propagating, diversifying organization.” Most profoundly, the mystery concerns the historical appearance since the big
```


## Search but Ignoring Case
less -i \
source: https://man7.org/linux/man-pages/man1/less.1.html
With the -i option, less will ignore case in path and file names
### example 1:
the relative path of target file is "written_2/travel_guides/berlitz2/PuertoRico-History.txt", we alter the cases in a few places of this path, with the -i option, we are still able to reach our target file.
```
input:
$ less -i Written_2/Travel_guides/berLitz2/paris-whereTogo.txt

output:



Where To GoGetting AroundThe first thing you should get is a carnet, or book of ten métro tickets (good for buses, too). Or, better still, if you’re staying a week or more, one of the special passes which give even greater savings (see page 118). Then, buy a Museum Pass (see page 74) to save money and avoid waiting at ticket counters.To get your bearings, picture Paris as a circle, with the river Seine threading across the center, flanked by famous landmarks — Notre-Dame, the Louvre, place de la Concorde, Arc de Triomphe, the Tour Eiffel. Bridges link the Right (north) and Left Banks via the two islands in the middle, Ile de la Cité and Ile St-Louis.This is one of the easiest of large cities to travel around. The modernized métro system is smooth, regular, and fast, with low, flat-rate fares. RER commuter trains can also take you rapidly to the outskirts, where two major attractions, Versailles and the Disneyland Paris Resort, are located.Buses give you a sightseeing tour at a bargain price, respecting schedules as far as traffic allows (rush hours can create terrible jams). Taxis provide a lazy alternative, but are not always faster than the métro, especially on longer rides across town.Bus tours take you to the big attractions, but inevitably at times when they are busiest. Some tour buses that take you around the highlights let you hop on and off, wherever and as often as you like, all on one ticket, for a period of up to 48 hours. Tourist information offices (see page 121) have details. Bicycle rental companies (see page 103) also run tours. If you want to sightsee in style (and expensively) you can even see Paris from a helicopter, plane, or hot-air balloon. In-line skates have become very popular for touring the town and can also be rented (see page 103).Parisians themselves often use the Batobus (river bus) for traveling east or west and avoiding traffic snarls. It runs from May to September; stops are at the Tour Eiffel, Musée d’Orsay, Louvre, Notre-Dame, and Hôtel de Ville. It’s relatively expensive, but you may prefer the absence of commentary.A boat cruise on the Seine is one of the best introductions to the city. While you glide along, multilingual commentaries tell you about the sights. Boats run from about 10am to 10:30pm. Most tour boats provide a choice of open-air and glassed-in seating; some offer lunch and dinner. Trips last 60 to 75 minutes. Canal tours reveal a less grand but more intimate face of Paris on the way from the center to Parc de la Villette (see page 72) in the northeastern outskirts. The leisurely trip takes three hours, with a tunnel and several locks to be negotiated.Central Paris is surprisingly compact, and most hotels are close to many of the sights. So if time isn’t a major factor, the best way of getting the feel of the place is to walk. All you need is a pair of comfortable shoes and a map. The big department stores and hotels give away millions of street maps each year. Métro stations display good maps of their local district as well as the métro itself, and give out pocket plans of the métro and bus routes. At street level, bus-stop shelters have an excellent detailed map of the neighborhood. More and more streets and entire areas like Les Halles and Beaubourg have been pedestrianized, adding to the profusion of parks, squares, and gardens.The IslandsIle de la CitéThis is where Paris’s story began. Like the emblem on its coat of arms, the Ile de la Cité takes the form of a boat, with the romantic tree-shaded place du Vert Galant as its prow pointing downstream. From the first settlement built by the original Parisii until the middle of the 19th century, the pocket-sized island lay at the heart of the city. The earliest rulers held court here. The cathedral clergy and artisans made it their home. Then, ruthless urban planner Baron Haussmann swept away almost all the medieval and 17th-century structures, leaving just place Dauphine and rue Chanoinesse (ancient home of the cathedral canons) as signs of the island’s once rich residential life.The baron was also toying with the idea of replacing the gracious red brick houses of the triangular place Dauphine with a neo-Grecian colonnaded square when, thankfully, he was forced out of office for juggling the books. Near the lively Pont-Neuf, the place was built in 1607 by Henri IV in honor of his son the dauphin (or future king, Louis XIII). Sadly, only numbers 14 and 26 are still in their original state. Number 10 was the home of film stars Simone Signoret and Yves Montand.The huge Palais de Justice, heart of the centralized French legal system, stands on the site of the Roman palace where the Emperor Julian was crowned in 360. Together with the Conciergerie (see page 30), it sprawls right across the Ile de la Cité. Concealed in the courtyard between them is a Gothic masterpiece, the Sainte-Chapelle, whose fine proportions stand in sharp contrast to the ponderous palace. The chapel was constructed in 1248 to house holy relics, fragments of what were believed to be Jesus’s Crown of Thorns and the True Cross, which pious Louis IX (later canonized as St. Louis) had bought from the Byzantine emperor. Try to arrive as the chapel opens or at sunset (see page 39) and make your way to the upper level, where light blazes in through 15 stained-glass windows separated by buttresses so slim that there seems to be no wall at all. Miraculously, of the 1,134 individual pieces of glass, 720 are 13th-century originals. The chapel provides an exquisite setting for chamber music concerts.Between 1789 and 1815 the chapel assumed various guises: a flour warehouse during the Revolution and a club for high-ranking dandies, then an archive for Napoléon’s Consulate. It was this latter role that saved the chapel from projected destruction, since the bureaucrats could not think of another site in which to put their mountains of paper.
These days, they find room for their papers in the Palais de Justice and the nearby Préfecture de Police, haunt of those fictional detectives, Inspectors Maigret and Clouseau. The great lobby of the Palais, the Salle des Pas Perdus, is worth a visit for a glimpse of the many lawyers, plaintiffs, witnesses, court reporters, and assorted hangers-on waiting nervously for the wheels of French justice to grind into action.
```
### example 2:
use less -i to access files under current directory, which is prevent error message from typing the wrong case
```
$ ls
Algarve-History.txt      Athens-WhatToDo.txt    Barcelona-WhatToDo.txt   Bermuda-WhereToGo.txt     CanaryIslands-History.txt    CostaBlanca-WhatToDo.txt  Cuba-WhereToGo.txt      Portugal-WhatToDo.txt
Algarve-Intro.txt        Athens-WhereToGo.txt   Barcelona-WhereToGo.txt  Boston-WhereToGo.txt      CanaryIslands-WhatToDo.txt   Costa-History.txt         Nepal-History.txt       Portugal-WhereToGo.txt
Algarve-WhatToDo.txt     Bahamas-History.txt    Beijing-History.txt      Budapest-History.txt      CanaryIslands-WhereToGo.txt  Costa-WhatToDo.txt        Nepal-WhatToDo.txt      PuertoRico-History.txt        
Algarve-WhereToGo.txt    Bahamas-Intro.txt      Beijing-WhatToDo.txt     Budapest-WhatToDo.txt     Cancun-History.txt           Costa-WhereToGo.txt       Nepal-WhereToGo.txt     PuertoRico-WhatToDo.txt       
Amsterdam-History.txt    Bahamas-WhatToDo.txt   Beijing-WhereToGo.txt    Budapest-WhereoGo.txt     Cancun-WhatToDo.txt          Crete-History.txt         NewOrleans-History.txt  PuertoRico-WhereToGo.txt      
Amsterdam-Intro.txt      Bahamas-WhereToGo.txt  Berlin-History.txt       California-History.txt    Cancun-WhereToGo.txt         Crete-WhatToDo.txt        Paris-WhatToDo.txt      Vallarta-History.txt
Amsterdam-WhatToDo.txt   Bali-History.txt       Berlin-WhatToDo.txt      California-WhatToDo.txt   China-History.txt            Crete-WhereToGo.txt       Paris-WhereToGo.txt     Vallarta-WhatToDo.txt
Amsterdam-WhereToGo.txt  Bali-WhatToDo.txt      Berlin-WhereToGo.txt     California-WhereToGo.txt  China-WhatToDo.txt           CstaBlanca-WhereToGo.txt  Poland-History.txt      Vallarta-WhereToGo.txt        
Athens-History.txt       Bali-WhereToGo.txt     Bermuda-history.txt      Canada-History.txt        China-WhereToGo.txt          Cuba-History.txt          Poland-WhatToDo.txt
Athens-Intro.txt         Barcelona-History.txt  Bermuda-WhatToDo.txt     Canada-WhereToGo.txt      CostaBlanca-History.txt      Cuba-WhatToDo.txt         Portugal-History.txt

input: 
$ less -i cuba-whattodo.txt


output:
What to DoEntertainmentAlthough cultural activity has been under state control since the revolution and Havana no longer sizzles with the sleazy Mafia-funded casinos and clubs of the 1950s, both high culture and more down-to-earth nightlife thrive in Cuba. Outside the resorts, it can be hard to pin down what’s going on where, but informal musical performances are ubiquitous. In the resorts, nightlife is focused around hotels, ranging from decent live bands, dance, and fashion shows to mimed Beatles sing-a-longs.Live Music PerformancesCubans crave live music, and — with the surge in international popularity of traditional Cuban music — so do most visitors to Cuba. You certainly won’t have to go out of your way to hear music performances. Roving groups of musicians can be found playing everywhere from airports to restaurants. Merely wandering the streets of Havana, Santiago, or Trinidad, you’re likely to stumble across a party with a live band, or even a back alley where some impromptu jamming is going on. On Saturday nights in Camagüey, the music spreads to the streets in a “Noche Camagüeya” block party along Calle República.All the styles of Cuba’s delectable traditional music �� habaneras, son, boleros, guarachas, guajiras, and more — can be heard in every town’s casa de la trova, usually a fine old building on or near the main square. Performances are amateur and professional, take place afternoons and evenings, and are free or have a minimal cover charge (US$1–$2). Especially in the evenings and on weekends, when you’ll encounter a vibrant mix of Cubans and foreigners, the island’s casas de la trova really swing. The most famous is in Santiago de Cuba (which has sprung many a star), while those in towns like Trinidad, Baracoa, and Camagüey are especially charming.
Aside from traditional acoustic music, Cuba revels in salsa and jazz. Probably the best place for live jazz and salsa in the country is the rollicking Palacio de la Salsa, in Havana’s slightly dated Hotel Riviera (Paseo y Malecón, in Vedado; Tel. 33-4501). There, from midnight on, Cuba’s very best salsa bands perform (dancing is very much in order), and jazz artists entertain drinkers in the adjacent bar from Thursday to Sunday from 9pm.
Other music hotspots include:Havana. Casa de la Música (salsa; Avenida 35 and Calle 20, Miramar), Casa de la Trova (San Lázaro between Gervasio and Belascoán, Central Havana), and El Zorro y el Cuevo, (jazz; Calles 23 y O, Vedado).      Trinidad. Casa de la Trova (Hernández Echerrí, 29), Casa de la Música (Calle Márquez), La Canchánchara (Calle Villena, 70), and Casa Fisher (Calle Lino Pérez).
Santiago de Cuba. Casa de la Trova (Calle Heredia), Casa de las Tradiciones (Calle General Lacret).Baracoa. Casa de la Trova (José Martí, 149) and Casa de la Cultura (Maceo, 122).Cabaret
A legacy of the high-rolling casino days in Cuba, cabarets have been kept alive and well as an outlet for tourist dollars. Cavorting mulatta dancers in sparkling G-strings and pairs of strategically placed stars may not be most peoples’ image of socialist doctrine — but this is Caribbean communism. While the best shows (at the Tropicana clubs in both Havana and Santiago de Cuba) are rather expensive by Cuban standards, seeing at least one big song-and-dance production in the flesh (so to speak) is de riguer.
The Tropicana in Havana (Calles 72 and 43, Marianao; Tel. 33-7507), founded in 1939 in a dazzling open-air arena, is indisputably the queen of cabarets. The likes of Nat King Cole performed here in pre-revolutionary times. With a 32-piece orchestra and a cast of over 200 (some parading in impossibly large headdresses), the sheer scale of the spectacle will make your head spin. The show regularly kicks off at 9:30pm, and a shorter performance follows later; there are also a restaurant and disco. Reservations and transportation can be arranged at your hotel for US$60. You can always visit independently, but the venue, situated in the suburb of Marianao, is tricky to find, and you might arrive only to find no tickets remaining. Havana’s next-best cabaret show, smaller and less expensive, is Cabaret Parisien, at the Hotel Nacional (Calles 21 and O, Vedado; Tel. 30-3564), nightly at 10:30pm; admission is US$35.
The Tropicana in Santiago de Cuba (Autopista Nacional km 1.5, with signs from Plaza de la Revolución; Tel. 4-3036) fills an enormous, recently constructed complex on the city’s northern outskirts. It is no less impressive than Havana’s but a bit less gaudy. Admission is US$30, including a drink ($27 if purchased from a travel agency).
In Varadero, the Cabaret Continental at the Hotel Internacional (shows nightly from 8:30pm to 3am) pales in comparison with the former venues but is nonetheless an enjoyable and sometimes fairly raunchy song-and-dance extravaganza. A fun show — kind of Afro-Cuban with a pirate theme — followed by disco takes place in a cave at the Cueva del Pirata, some 9 km (6 miles) east of Varadero (Autopista Sur, km 11), nightly at 10:30pm until the wee hours. There is also a cabaret at the Meliá Varadero hotel.
Discos
Discos pulsate to both Latin and Euro-American rhythms. The places to be are Habana Café (the disco in Havana’s Hotel Meliá Cohiba) and the disco in Santiago’s eponymous hotel. These are glitzy affairs, where foreigners get soaked and approached by hustlers of all stripes. Also try El Galeón, in a make-believe pirate ship that sets sail from under Havana’s La Cabaña fortress. The best in Varadero is La Bamba at the Hotel Tuxpan (entrance US$10–$15). Also try the open-air Discoteca La Patana, near the bridge into Varadero. In Trinidad, Motel Las Cuevas has a disco with live entertainment, but it pales in comparison to the music halls in town. In Guardalavaca, head for open-air La Roca, set just above the beach.
Bars and Cafés
```

## Show Where Are We At When Viewing a File
less -mouse \
source: https://man7.org/linux/man-pages/man1/less.1.html
### example1:
use less -mouse when viewing file, give us more clue where are we at on a file
```
input: 
$ less -mouse -i cuba-whattodo.txt

output:
What to DoEntertainment
Although cultural activity has been under state control since the revolution and Havana no longer sizzles with the sleazy Mafia-funded casinos and clubs of the 1950s, both high culture and more down-to-earth nightlife thrive in Cuba. Outside the resorts, it can be hard to pin down what’s going on where, but informal musical performances are ubiquitous. In the resorts, nightlife is focused around hotels, ranging from decent live bands, dance, and fashion shows to mimed Beatles sing-a-longs.
Live Music PerformancesCubans crave live music, and — with the surge in international popularity of traditional Cuban music — so do most visitors to Cuba. You certainly won’t have to go out of your way to hear music performances. Roving groups of musicians can be found playing everywhere from airports to restaurants. Merely wandering the streets of Havana, Santiago, or Trinidad, you’re likely to stumble across a party with a live band, or even a back alley where some impromptu jamming is going on. On Saturday nights in Camagüey, the music spreads to the streets in a “Noche Camagüeya” block party along Calle República.
All the styles of Cuba’s delectable traditional music �� habaneras, son, boleros, guarachas, guajiras, and more — can be heard in every town’s casa de la trova, usually a fine old building on or near the main square. Performances are amateur and professional, take place afternoons and evenings, and are free or have a minimal cover charge (US$1–$2). Especially in the evenings and on weekends, when you’ll encounterCuba-History.txtCuba-WhatToDo.txt
Cuba-WhereToGo.txt




What to Do
Entertainment
Although cultural activity has been under state control since the revolution and Havana no longer sizzles with the sleazy Mafia-funded casinos and clubs of the 1950s, both high culture and more down-to-earth nightlife thrive in Cuba. Outside the resorts, it can be hard to pin down what’s going on where, but informal musical performances are ubiquitous. In the resorts, nightlife is focused around hotels, ranging from decent live bands, dance, and fashion shows to mimed Beatles sing-a-longs.Live Music PerformancesCubans crave live music, and — with the surge in international popularity of traditional Cuban music — so do most visitors to Cuba. You certainly won’t have to go out of your way to hear music performances. Roving groups of musicians can be found playing everywhere from airports to restaurants. Merely wandering the streets of Havana, Santiago, or Trinidad, you’re likely to stumble across a party with a live band, or even a back alley where some impromptu jamming is going on. On Saturday nights in Camagüey, the music spreads to the streets in a “Noche Camagüeya” block party along Calle República.All the styles of Cuba’s delectable traditional music �� habaneras, son, boleros, guarachas, guajiras, and more — can be heard in every town’s casa de la trova, usually a fine old building on or near the main square. Performances are amateur and professional, take place afternoons and evenings, and are free or have a minimal cover charge (US$1–$2). Especially in the evenings and on weekends, when you’ll encounter a vibrant mix of Cubans and foreigners, the island’s casas de la trova really swing. The most famous is in Santiago de Cuba (which has sprung many a star), while those in towns like Trinidad, Baracoa, and Camagüey are especially charming.Aside from traditional acoustic music, Cuba revels in salsa and jazz. Probably the best place for live jazz and salsa in the country is the rollicking Palacio de la Salsa, in Havana’s slightly dated Hotel Riviera (Paseo y Malecón, in Vedado; Tel. 33-4501). There, from midnight on, Cuba’s very best salsa bands perform (dancing is very much in order), and jazz artists entertain drinkers in the adjacent bar from Thursday to Sunday from 9pm.Other music hotspots include:
Havana. Casa de la Música (salsa; Avenida 35 and Calle 20, Miramar), Casa de la Trova (San Lázaro between Gervasio and Belascoán, Central Havana), and El Zorro y el Cuevo, (jazz; Calles 23 y O, Vedado).      
Trinidad. Casa de la Trova (Hernández Echerrí, 29), Casa de la Música (Calle Márquez), La Canchánchara (Calle Villena, 70), and Casa Fisher (Calle Lino Pérez).Santiago de Cuba. Casa de la Trova (Calle Heredia), Casa de las Tradiciones (Calle General Lacret).
Baracoa. Casa de la Trova (José Martí, 149) and Casa de la Cultura (Maceo, 122).Cabaret
A legacy of the high-rolling casino days in Cuba, cabarets have been kept alive and well as an outlet for tourist dollars. Cavorting mulatta dancers in sparkling G-strings and pairs of strategically placed stars may not be most peoples’ image of socialist doctrine — but this is Caribbean communism. While the best shows (at the Tropicana clubs in both Havana and Santiago de Cuba) are rather expensive by Cuban standards, seeing at least one big song-and-dance production in the flesh (so to speak) is de riguer.The Tropicana in Havana (Calles 72 and 43, Marianao; Tel. 33-7507), founded in 1939 in a dazzling open-air arena, is indisputably the queen of cabarets. The likes of Nat King Cole performed here in pre-revolutionary times. With a 32-piece orchestra and a cast of over 200 (some parading in impossibly large headdresses), the sheer scale of the spectacle will make your head spin. The show regularly kicks off at 9:30pm, and a shorter performance follows later; there are also a restaurant and disco. Reservations and transportation can be arranged at your hotel for US$60. You can always visit independently, but the venue, situated in the suburb of Marianao, is tricky to find, and you might arrive only to find no tickets remaining. Havana’s next-best cabaret show, smaller and less expensive, is Cabaret Parisien, at the Hotel Nacional (Calles 21 and O, Vedado; Tel. 30-3564), nightly at 10:30pm; admission is US$35.
The Tropicana in Santiago de Cuba (Autopista Nacional km 1.5, with signs from Plaza de la Revolución; Tel. 4-3036) fills an enormous, recently constructed complex on the city’s northern outskirts. It is no less impressive than Havana’s but a bit less gaudy. Admission is US$30, including a drink ($27 if purchased from a travel agency).
In Varadero, the Cabaret Continental at the Hotel Internacional (shows nightly from 8:30pm to 3am) pales in comparison with the former venues but is nonetheless an enjoyable and sometimes fairly raunchy song-and-dance extravaganza. A fun show — kind of Afro-Cuban with a pirate theme — followed by disco takes place in a cave at the Cueva del Pirata, some 9 km (6 miles) east of Varadero (Autopista Sur, km 11), nightly at 10:30pm until the wee hours. There is also a cabaret at the Meliá Varadero hotel.
DiscosDiscos pulsate to both Latin and Euro-American rhythms. The places to be are Habana Café (the disco in Havana’s Hotel Meliá Cohiba) and the disco in Santiago’s eponymous hotel. These are glitzy affairs, where foreigners get soaked and approached by hustlers of all stripes. Also try El Galeón, in a make-believe pirate ship that sets sail from under Havana’s La Cabaña fortress. The best in Varadero is La Bamba at the Hotel Tuxpan (entrance US$10–$15). Also try the open-air Discoteca La Patana, near the bridge into Varadero. In Trinidad, Motel Las Cuevas has a disco with live entertainment, but it pales in comparison to the music halls in town. In Guardalavaca, head for open-air La Roca, set just above the beach.
Bars and Cafés
cuba-whattodo.txt 35%

```

### example 2:

a very similar command less -MOUSE give use a little bit more information, other than showing what percentage have we view, also tell us which line of the file are we at
```
input:
$ less -MOUSE -i cuba-whattodo.txt

output:
What to DoEntertainmentAlthough cultural activity has been under state control since the revolution and Havana no longer sizzles with the sleazy Mafia-funded casinos and clubs of the 1950s, both high culture and more down-to-earth nightlife thrive in Cuba. Outside the resorts, it can be hard to pin down what’s going on where, but informal musical performances are ubiquitous. In the resorts, nightlife is focused around hotels, ranging from decent live bands, dance, and fashion shows to mimed Beatles sing-a-longs.
Live Music PerformancesCubans crave live music, and — with the surge in international popularity of traditional Cuban music — so do most visitors to Cuba. You certainly won’t have to go out of your way to hear music performances. Roving groups of musicians can be found playing everywhere from airports to restaurants. Merely wandering the streets of Havana, Santiago, or Trinidad, you’re likely to stumble across a party with a live band, or even a back alley where some impromptu jamming is going on. On Saturday nights in Camagüey, the music spreads to the streets in a “Noche Camagüeya” block party along Calle República.All the styles of Cuba’s delectable traditional music �� habaneras, son, boleros, guarachas, guajiras, and more — can be heard in every town’s casa de la trova, usually a fine old building on or near the main square. Performances are amateur and professional, take place afternoons and evenings, and are free or have a minimal cover charge (US$1–$2). Especially in the evenings and on weekends, when you’ll encounter a vibrant mix of Cubans and foreigners, the island’s casas de la trova really swing. The most famous is in Santiago de Cuba (which has sprung many a star), while those in towns like Trinidad, Baracoa, and Camagüey are especially charming.Aside from traditional acoustic music, Cuba revels in salsa and jazz. Probably the best place for live jazz and salsa in the country is the rollicking Palacio de la Salsa, in Havana’s slightly dated Hotel Riviera (Paseo y Malecón, in Vedado; Tel. 33-4501). There, from midnight on, Cuba’s very best salsa bands perform (dancing is very much in order), and jazz artists entertain drinkers in the adjacent bar from Thursday to Sunday from 9pm.Other music hotspots include:
Havana. Casa de la Música (salsa; Avenida 35 and Calle 20, Miramar), Casa de la Trova (San Lázaro between Gervasio and Belascoán, Central Havana), and El Zorro y el Cuevo, (jazz; Calles 23 y O, Vedado).      Trinidad. Casa de la Trova (Hernández Echerrí, 29), Casa de la Música (Calle Márquez), La Canchánchara (Calle Villena, 70), and Casa Fisher (Calle Lino Pérez).
Santiago de Cuba. Casa de la Trova (Calle Heredia), Casa de las Tradiciones (Calle General Lacret).
Baracoa. Casa de la Trova (José Martí, 149) and Casa de la Cultura (Maceo, 122).CabaretA legacy of the high-rolling casino days in Cuba, cabarets have been kept alive and well as an outlet for tourist dollars. Cavorting mulatta dancers in sparkling G-strings and pairs of strategically placed stars may not be most peoples’ image of socialist doctrine — but this is Caribbean communism. While the best shows (at the Tropicana clubs in both Havana and Santiago de Cuba) are rather expensive by Cuban standards, seeing at least one big song-and-dance production in the flesh (so to speak) is de riguer.
The Tropicana in Havana (Calles 72 and 43, Marianao; Tel. 33-7507), founded in 1939 in a dazzling open-air arena, is indisputably the queen of cabarets. The likes of Nat King Cole performed here in pre-revolutionary times. With a 32-piece orchestra and a cast of over 200 (some parading in impossibly large headdresses), the sheer scale of the spectacle will make your head spin. The show regularly kicks off at 9:30pm, and a shorter performance follows later; there are also a restaurant and disco. Reservations and transportation can be arranged at your hotel for US$60. You can always visit independently, but the venue, situated in the suburb of Marianao, is tricky to find, and you might arrive only to find no tickets remaining. Havana’s next-best cabaret show, smaller and less expensive, is Cabaret Parisien, at the Hotel Nacional (Calles 21 and O, Vedado; Tel. 30-3564), nightly at 10:30pm; admission is US$35.
The Tropicana in Santiago de Cuba (Autopista Nacional km 1.5, with signs from Plaza de la Revolución; Tel. 4-3036) fills an enormous, recently constructed complex on the city’s northern outskirts. It is no less impressive than Havana’s but a bit less gaudy. Admission is US$30, including a drink ($27 if purchased from a travel agency).
In Varadero, the Cabaret Continental at the Hotel Internacional (shows nightly from 8:30pm to 3am) pales in comparison with the former venues but is nonetheless an enjoyable and sometimes fairly raunchy song-and-dance extravaganza. A fun show — kind of Afro-Cuban with a pirate theme — followed by disco takes place in a cave at the Cueva del Pirata, some 9 km (6 miles) east of Varadero (Autopista Sur, km 11), nightly at 10:30pm until the wee hours. There is also a cabaret at the Meliá Varadero hotel.
Discos
Discos pulsate to both Latin and Euro-American rhythms. The places to be are Habana Café (the disco in Havana’s Hotel Meliá Cohiba) and the disco in Santiago’s eponymous hotel. These are glitzy affairs, where foreigners get soaked and approached by hustlers of all stripes. Also try El Galeón, in a make-believe pirate ship that sets sail from under Havana’s La Cabaña fortress. The best in Varadero is La Bamba at the Hotel Tuxpan (entrance US$10–$15). Also try the open-air Discoteca La Patana, near the bridge into Varadero. In Trinidad, Motel Las Cuevas has a disco with live entertainment, but it pales in comparison to the music halls in town. In Guardalavaca, head for open-air La Roca, set just above the beach.
Bars and Cafés
cuba-whattodo.txt lines 1-24/56 35%

```

##  Combine less with Other Command by Pipe
other command | less \
source: https://www.geeksforgeeks.org/less-command-linux-examples/
### example 1:
view result from the find command immediately by joining the less command with a pipe. Combine with the -N option in less command, we can quickly tell how many subdirectories and files did the find command return

```
input:
find written_2/ | less -N

output:
      1 written_2/
      2 written_2/non-fiction
      3 written_2/non-fiction/OUP
      4 written_2/non-fiction/OUP/Abernathy
      5 written_2/non-fiction/OUP/Abernathy/ch1.txt
      6 written_2/non-fiction/OUP/Abernathy/ch14.txt
      7 written_2/non-fiction/OUP/Abernathy/ch15.txt
      8 written_2/non-fiction/OUP/Abernathy/ch2.txt
      9 written_2/non-fiction/OUP/Abernathy/ch3.txt
     10 written_2/non-fiction/OUP/Abernathy/ch6.txt
     11 written_2/non-fiction/OUP/Abernathy/ch7.txt
     12 written_2/non-fiction/OUP/Abernathy/ch8.txt
     13 written_2/non-fiction/OUP/Abernathy/ch9.txt
     14 written_2/non-fiction/OUP/Berk
     15 written_2/non-fiction/OUP/Berk/ch1.txt
     16 written_2/non-fiction/OUP/Berk/ch2.txt
     17 written_2/non-fiction/OUP/Berk/CH4.txt
     18 written_2/non-fiction/OUP/Berk/ch7.txt
     19 written_2/non-fiction/OUP/Castro
     20 written_2/non-fiction/OUP/Castro/chA.txt
     21 written_2/non-fiction/OUP/Castro/chB.txt
     22 written_2/non-fiction/OUP/Castro/chC.txt
     23 written_2/non-fiction/OUP/Castro/chL.txt
     24 written_2/non-fiction/OUP/Castro/chM.txt
     25 written_2/non-fiction/OUP/Castro/chN.txt
     26 written_2/non-fiction/OUP/Castro/chO.txt
     27 written_2/non-fiction/OUP/Castro/chP.txt
     28 written_2/non-fiction/OUP/Castro/chQ.txt
     29 written_2/non-fiction/OUP/Castro/chR.txt
     30 written_2/non-fiction/OUP/Castro/chV.txt
     31 written_2/non-fiction/OUP/Castro/chW.txt
     32 written_2/non-fiction/OUP/Castro/chY.txt
     33 written_2/non-fiction/OUP/Castro/chZ.txt
     34 written_2/non-fiction/OUP/Fletcher
     35 written_2/non-fiction/OUP/Fletcher/ch1.txt
     36 written_2/non-fiction/OUP/Fletcher/ch10.txt
     37 written_2/non-fiction/OUP/Fletcher/ch2.txt
     38 written_2/non-fiction/OUP/Fletcher/ch5.txt
     39 written_2/non-fiction/OUP/Fletcher/ch6.txt
     40 written_2/non-fiction/OUP/Fletcher/ch9.txt
     41 written_2/non-fiction/OUP/Kauffman
     42 written_2/non-fiction/OUP/Kauffman/ch1.txt
     43 written_2/non-fiction/OUP/Kauffman/ch10.txt
     44 written_2/non-fiction/OUP/Kauffman/ch3.txt
     45 written_2/non-fiction/OUP/Kauffman/ch4.txt
:
```
### example 2:


