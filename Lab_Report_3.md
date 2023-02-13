# The Grep Command

**Definition**

Grep, which is short for "global regular expression print," is a command that is used to searching for a regular expression or string in a .txt file.

# Command Line options

Each command will use a pattern.
This pattern is used to search the subdirectories in ./written_2.

## Number 1: -l

-l is used to only show matching files in the output only.

**Example 1**

    bdikbas@Buraks-MacBook-Pro written_2 % grep -l "Lucayans" */*/*.txt
    travel_guides/berlitz2/Bahamas-History.txt
    
**Example 2**

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

The -l is useful because it allows use to figure out which file contains the string that we are looking for.

[Link] (https://en.wikibooks.org/wiki/Grep)

## Number 2: -h

-h is used to Output the lines that match the string, but not the actual file.

**Example 1**

    bdikbas@Buraks-MacBook-Pro written_2 % grep -h "Lucayans" */*/*.txt
    Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. 
    Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught       from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the 
    Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. 
    We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and     other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
    
    The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the             archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — 
    at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to     Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from 
    the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

**Example 2**
    
    bdikbas@Buraks-MacBook-Pro written_2 % grep -h "The Bahamas has a number of PGA-level" */*/*.txt
    The Bahamas has a number of PGA-level courses. Grand Bahama has the well tended Lucaya Golf and Country Club (Tel. 373-1066), 
    and the Bahamas Princess Golf and Country Club, part of the Bahamas Princess Complex at Freeport, has two courses (Tel. 352-6721) 
    both designed by Dick Wilson. New Providence has Paradise Island Golf Club (Tel. 363-3925) and one at Cable Beach (Tel. 327-6000). 
    On Abaco Island, Treasure Beach has an 18-hole course (Tel. 365-8045).
    
The first command is used to find the .txt files that contain the string "Lucayans". With the -h command, it doesn't print the file that the string is in, rather the line that it is on.

The second command is used to find the .txt files that contain the string "The Bahamas has a number of PGA-level". With the help of the -h command, it only shows the lines that the string is contained.

The -h is useful because it allows us to see the line that contains the string if we do not need the file.

## Number 3: -o

-o is used to only output the matching strings in the lines inside the files that contain the string.

**Example 1**

    bdikbas@Buraks-MacBook-Pro written_2 % grep -o "The Bahamas has a number of PGA-level" */*/*.txt
    travel_guides/berlitz2/Bahamas-WhatToDo.txt:The Bahamas has a number of PGA-level
    
**Example 2**

    bdikbas@Buraks-MacBook-Pro written_2 % grep -o "Lucayans" */*/*.txt                     
    travel_guides/berlitz2/Bahamas-History.txt:Lucayans
    travel_guides/berlitz2/Bahamas-History.txt:Lucayans

The first command is used to find the .txt files that contain the string "The Bahamas has a number of PGA-level". With -o, it only shows the output of that string the amount of times that it shows up in that file, which in this case, would be 1.

The second command is used to find the .txt files that contain the string "Lucayans". With -o, it only shows the string based on how often it shows up in all the files, which would be 2.

The -o command is useful because it shows us the file that contains the string and the string itself that we were trying to find.

## Number 4: -n

-n has each matching line precede with a line number. This line number is the line in the file that contains the string. The whole line is also printed.

**Example 1**

        bdikbas@Buraks-MacBook-Pro written_2 % grep -n "Lucayans" */*/*.txt
        travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the 
        Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by 
        cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them 
        for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East 
        Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for 
        his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
        
        travel_guides/berlitz2/Bahamas-History.txt:7:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that 
        their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On 
        Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on 
        their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years 
        all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl 
        fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
        
**Example 2**

        bdikbas@Buraks-MacBook-Pro written_2 % grep -n "The Bahamas has a number of PGA-level" */*/*.txt
        travel_guides/berlitz2/Bahamas-WhatToDo.txt:48:The Bahamas has a number of PGA-level courses. Grand Bahama has the well tended Lucaya Golf and 
        Country Club (Tel. 373-1066), and the Bahamas Princess Golf and Country Club, part of the Bahamas Princess Complex at Freeport, has two courses 
        (Tel. 352-6721) both designed by Dick Wilson. New Providence has Paradise Island Golf Club (Tel. 363-3925) and one at Cable Beach (Tel. 327-
        6000). On Abaco Island, Treasure Beach has an 18-hole course (Tel. 365-8045).

The first command is used to find the string "Lucayans". With -n, it prints the two lines that the string is found on (Lines 6 & 7) in addition to the line numbers before the line (6: the entire line & 7: the entire line).

The second command is used to find the string "The Bahamas has a number of PGA-level". With -n, it prints line 48 in the Bahamas-WhatToDo.txt file, which contains the string that we are trying to search for.

-n is useful to use because it shows us the file where the string is, the line number that the string is in, and the entire line.
