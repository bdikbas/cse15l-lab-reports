# The Grep Command

**Definition**

Grep, which is short for "global regular expression print," is a command that is used to searching for a regular expression or string in a .txt file.

# Command Line options

## Number 1: -l

-l is used to only show matching files in the output only.


    bdikbas@Buraks-MacBook-Pro written_2 % grep -l "Lucayans" */*/*.txt
    travel_guides/berlitz2/Bahamas-History.txt
    
    bdikbas@Buraks-MacBook-Pro written_2 % grep -l "Italy" */*/*.txt
    travel_guides/berlitz1/HistoryFrance.txt
    travel_guides/berlitz1/HistoryGreek.txt
    travel_guides/berlitz1/HistoryIstanbul.txt
    travel_guides/berlitz1/HistoryItaly.txt
    travel_guides/berlitz1/HistoryMadeira.txt
    travel_guides/berlitz1/HistoryMallorca.txt
    travel_guides/berlitz1/IntroItaly.txt
    travel_guides/berlitz1/IntroLasVegas.txt
    travel_guides/berlitz1/WhatToItaly.txt
    travel_guides/berlitz1/WhereToEgypt.txt
    travel_guides/berlitz1/WhereToFWI.txt
    travel_guides/berlitz1/WhereToFrance.txt
    travel_guides/berlitz1/WhereToGreek.txt
    travel_guides/berlitz1/WhereToIstanbul.txt
    travel_guides/berlitz1/WhereToItaly.txt
    travel_guides/berlitz1/WhereToMadrid.txt
    travel_guides/berlitz2/Algarve-History.txt
    travel_guides/berlitz2/Athens-History.txt
    travel_guides/berlitz2/Athens-WhatToDo.txt
    travel_guides/berlitz2/Barcelona-WhereToGo.txt
    travel_guides/berlitz2/California-WhereToGo.txt
    travel_guides/berlitz2/Canada-History.txt
    travel_guides/berlitz2/Canada-WhereToGo.txt
    travel_guides/berlitz2/Costa-History.txt
    travel_guides/berlitz2/CostaBlanca-History.txt
    travel_guides/berlitz2/Crete-WhereToGo.txt
    travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
    travel_guides/berlitz2/Paris-WhereToGo.txt
    travel_guides/berlitz2/Portugal-History.txt
    travel_guides/berlitz2/Portugal-WhatToDo.txt
    
The first command is used to find the .txt files that contain the string "Lucayans". When the command is ran, it prints out the files that contains that that string.

The second command is used to find the .txt files that contain the string "Italy". When the command is ran, it prints out all the files that contains that string.

[Link] (https://en.wikibooks.org/wiki/Grep)

## Number 2: -h

-h is used to Output the lines that match the string, but not the actual file.

    bdikbas@Buraks-MacBook-Pro written_2 % grep -h "Lucayans" */*/*.txt
    Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. 
    Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught       from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the 
    Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. 
    We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and     other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
    
    The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the             archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — 
    at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to     Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from 
    the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

