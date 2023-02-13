# Less Command Options in Linux
 The less command shows a file (or files) contents one screen at a time, use q to quit the pager mode.

## Display Line Number with Less
less - N \
source: https://linuxhandbook.com/less-command/
### example 1:
We use less to access the content of a file, and the -N option show the line number of the content of the txt file, which give use and idea of how the content was organized.
```
input: 
  less -N written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
  
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
less -N written_2/travel_guides/berlitz1/HandRHawaii.txt written_2/non-fiction/OUP/Kauffman/ch4.txt

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


## Cause Search to Ignore Case
less -i \
source: https://man7.org/linux/man-pages/man1/less.1.html

## Highlight the String Which was found by Last Search Command
less -g \
source: https://man7.org/linux/man-pages/man1/less.1.html

##  Combine less with Other Command by Pipe
other command | less \
source: https://www.geeksforgeeks.org/less-command-linux-examples/



skill-demo1-data\written_2\non-fiction\OUP\Abernathy
