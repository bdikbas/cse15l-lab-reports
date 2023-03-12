# Lab Report 5

In Lab this week, we searched for and corrected different errors in student's code so that they would produce the correct results. There were 4 errors and each one had their own error, such as a command typed in the terminal incorrectly and even commands not being properly typed.
In this Lab report, we are supposed to go back to a previous lab and do it differntly than done in the past after learning all the different commands.

## Lab Report 3

In Lab Report 3, I found information on how to utilize the grep command and some of its command-line options.

## Command Line options

Each command will use a pattern.
This pattern is used to search the subdirectories in ./written_2.

## -c

-c is a command-line option that only prints the number of lines that match a pattern. The following Code is shortened due to how long the output was, so not all the results will be shown.
 
### Example 1

    bdikbas@Buraks-MacBook-Pro written_2 %  grep -c "Italy" */*/*.txt
    travel_guides/berlitz1/HandRHawaii.txt:0
    travel_guides/berlitz1/HandRHongKong.txt:0
    travel_guides/berlitz1/HandRIbiza.txt:0
    travel_guides/berlitz1/HandRIsrael.txt:0
    travel_guides/berlitz1/HandRIstanbul.txt:0
    travel_guides/berlitz1/HandRJamaica.txt:0
    travel_guides/berlitz1/HandRJerusalem.txt:0
    travel_guides/berlitz1/HandRLakeDistrict.txt:0
    travel_guides/berlitz1/HandRLasVegas.txt:0
    travel_guides/berlitz1/HandRLisbon.txt:0
    travel_guides/berlitz1/HandRLosAngeles.txt:0
    travel_guides/berlitz1/HandRMadeira.txt:0
    travel_guides/berlitz1/HandRMadrid.txt:0
    travel_guides/berlitz1/HandRMallorca.txt:0
    travel_guides/berlitz1/HistoryDublin.txt:0
    travel_guides/berlitz1/HistoryEdinburgh.txt:0
    travel_guides/berlitz1/HistoryEgypt.txt:0
    travel_guides/berlitz1/HistoryFWI.txt:0
    travel_guides/berlitz1/HistoryFrance.txt:3
    travel_guides/berlitz1/HistoryGreek.txt:1
    travel_guides/berlitz1/HistoryHawaii.txt:0
    travel_guides/berlitz1/HistoryHongKong.txt:0
    travel_guides/berlitz1/HistoryIbiza.txt:0
    travel_guides/berlitz1/HistoryIndia.txt:0
    travel_guides/berlitz1/HistoryIsrael.txt:0
    travel_guides/berlitz1/HistoryIstanbul.txt:2
    travel_guides/berlitz1/HistoryItaly.txt:44
    travel_guides/berlitz1/HistoryJamaica.txt:0
    travel_guides/berlitz1/HistoryJapan.txt:0
    travel_guides/berlitz1/HistoryJerusalem.txt:0
    travel_guides/berlitz1/HistoryLakeDistrict.txt:0
    travel_guides/berlitz1/HistoryLasVegas.txt:0
    travel_guides/berlitz1/HistoryMadeira.txt:1
    travel_guides/berlitz1/HistoryMadrid.txt:0
    travel_guides/berlitz1/HistoryMalaysia.txt:0
    travel_guides/berlitz1/HistoryMallorca.txt:1
    travel_guides/berlitz1/IntroDublin.txt:0
    travel_guides/berlitz1/IntroEdinburgh.txt:0
    travel_guides/berlitz1/IntroEgypt.txt:0
    travel_guides/berlitz1/IntroFWI.txt:0
    travel_guides/berlitz1/IntroFrance.txt:0
    travel_guides/berlitz1/IntroGreek.txt:0
    travel_guides/berlitz1/IntroHongKong.txt:0
    travel_guides/berlitz1/IntroIbiza.txt:0
    travel_guides/berlitz1/IntroIndia.txt:0
    travel_guides/berlitz1/IntroIsrael.txt:0
    travel_guides/berlitz1/IntroIstanbul.txt:0
    travel_guides/berlitz1/IntroItaly.txt:8
    travel_guides/berlitz1/IntroJamaica.txt:0
    travel_guides/berlitz1/IntroJapan.txt:0
    travel_guides/berlitz1/IntroJerusalem.txt:0
    travel_guides/berlitz1/IntroLakeDistrict.txt:0
    travel_guides/berlitz1/IntroLasVegas.txt:1
    travel_guides/berlitz1/IntroLosAngeles.txt:0
    travel_guides/berlitz1/IntroMadeira.txt:0
    travel_guides/berlitz1/IntroMadrid.txt:0
    travel_guides/berlitz1/IntroMalaysia.txt:0
    travel_guides/berlitz1/IntroMallorca.txt:0
    travel_guides/berlitz1/JungleMalaysia.txt:0
    travel_guides/berlitz1/WhatToDublin.txt:0
    travel_guides/berlitz1/WhatToEdinburgh.txt:0
    travel_guides/berlitz1/WhatToEgypt.txt:0
    travel_guides/berlitz1/WhatToFWI.txt:0
    travel_guides/berlitz1/WhatToFrance.txt:0
    travel_guides/berlitz1/WhatToGreek.txt:0
    travel_guides/berlitz1/WhatToHawaii.txt:0
    travel_guides/berlitz1/WhatToHongKong.txt:0
    travel_guides/berlitz1/WhatToIbiza.txt:0
    travel_guides/berlitz1/WhatToIndia.txt:0
    travel_guides/berlitz1/WhatToIsrael.txt:0
    travel_guides/berlitz1/WhatToIstanbul.txt:0
    travel_guides/berlitz1/WhatToItaly.txt:8
    travel_guides/berlitz1/WhatToJamaica.txt:0
    travel_guides/berlitz1/WhatToJapan.txt:0
    travel_guides/berlitz1/WhatToLakeDistrict.txt:0
    travel_guides/berlitz1/WhatToLasVegas.txt:0
    travel_guides/berlitz1/WhatToLosAngeles.txt:0
    travel_guides/berlitz1/WhatToMadeira.txt:0
    travel_guides/berlitz1/WhatToMalaysia.txt:0
    travel_guides/berlitz1/WhatToMallorca.txt:0
    travel_guides/berlitz1/WhereToDublin.txt:0
    travel_guides/berlitz1/WhereToEdinburgh.txt:0
    travel_guides/berlitz1/WhereToEgypt.txt:1
    travel_guides/berlitz1/WhereToFWI.txt:1
    travel_guides/berlitz1/WhereToFrance.txt:1
    travel_guides/berlitz1/WhereToGreek.txt:2
        
### Example 2

    bdikbas@Buraks-MacBook-Pro written_2 % grep -c "Lucayans" */*/*.txt 
    travel_guides/berlitz1/HandRHawaii.txt:0
    travel_guides/berlitz1/HandRHongKong.txt:0
    travel_guides/berlitz1/HandRIbiza.txt:0
    travel_guides/berlitz1/HandRIsrael.txt:0
    travel_guides/berlitz1/HandRIstanbul.txt:0
    travel_guides/berlitz1/HandRJamaica.txt:0
    travel_guides/berlitz1/HandRJerusalem.txt:0
    travel_guides/berlitz1/HandRLakeDistrict.txt:0
    travel_guides/berlitz1/HandRLasVegas.txt:0
    travel_guides/berlitz1/HandRLisbon.txt:0
    travel_guides/berlitz1/HandRLosAngeles.txt:0
    travel_guides/berlitz1/HandRMadeira.txt:0
    travel_guides/berlitz1/HandRMadrid.txt:0
    travel_guides/berlitz1/HandRMallorca.txt:0
    travel_guides/berlitz1/HistoryDublin.txt:0
    travel_guides/berlitz1/HistoryEdinburgh.txt:0
    travel_guides/berlitz1/HistoryEgypt.txt:0
    travel_guides/berlitz1/HistoryFWI.txt:0
    travel_guides/berlitz1/HistoryFrance.txt:0
    travel_guides/berlitz1/HistoryGreek.txt:0
    travel_guides/berlitz1/HistoryHawaii.txt:0
    travel_guides/berlitz1/HistoryHongKong.txt:0
    travel_guides/berlitz1/HistoryIbiza.txt:0

The first command is used to find the .txt files that contain the string "Italy". When the command is ran, it prints out the the number of lines that contain the string in each file.

The second command is used to find the .txt files that contain the string "Lucayans". When the command is ran, t prints out the the number of lines that contain the string in each file.

The -c is useful because it allows us to see the amount of lines that show the string in each file.

[Source](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## -w

-w is used to match the whole word.

### Example 1

    bdikbas@Buraks-MacBook-Pro written_2 % grep -w "Lucayans" */*/*.txt
    travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
    travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
    
### Example 2

    bdikbas@Buraks-MacBook-Pro written_2 % grep -w "The Bahamas" */*/*.txt 
    travel_guides/berlitz2/Bahamas-Intro.txt:The Bahamas and the Bahamians
    travel_guides/berlitz2/Bahamas-Intro.txt:The Bahamas islands are the flattened peaks of a huge ancient mountain range that once towered many thousands of feet into the sky. They now lie low in the water, the highest point — Mount Alvernia on Cat Island — being only 206 ft (65 m) above sea level. The eastern coastlines of the islands break the long tidal fetch that travels across the Atlantic; on the sheltered western coastline, coral outcrops have produced vast shallow sand banks that reflect waters of myriad translucent blues and greens.
    travel_guides/berlitz2/Bahamas-WhatToDo.txt:The Bahamas Sports and Aviation Information Centre provides complete information about sports facilities in the Bahamas. Call them toll-free at 800-32-SPORT (within the US only) or at 305-932-0051, or write for information to 19495 Biscayne Boulevard, Suite 809, Aventura, Florida 33180, USA.
    travel_guides/berlitz2/Bahamas-WhatToDo.txt:The Bahamas has a number of PGA-level courses. Grand Bahama has the well tended Lucaya Golf and Country Club (Tel. 373-1066), and the Bahamas Princess Golf and Country Club, part of the Bahamas Princess Complex at Freeport, has two courses (Tel. 352-6721) both designed by Dick Wilson. New Providence has Paradise Island Golf Club (Tel. 363-3925) and one at Cable Beach (Tel. 327-6000). On Abaco Island, Treasure Beach has an 18-hole course (Tel. 365-8045).
    travel_guides/berlitz2/Bahamas-WhereToGo.txt:The Bahamas has traditionally been divided into three entities: New Providence, Grand Bahama, and all the rest of the islands, brought together under the collective name of the Out Islands, sometimes also referred to as the Family Islands. Most of the Out Islands are sparsely populated, and the traditional ways of island life are much more prevalent than they are on the two main islands. The rhythm of life is slower, communities are smaller, and time seems to stand still. What activity there is centers around the boats that continually move quietly in and out of the harbors.
    
The first command is used to find the .txt files that contain the string "Lucayans". When the command is ran, it prints out the the lines that contains the whole word in addition to the file that contains it.

The second command is used to find the .txt files that contain the string "The Bahamas". When the command is ran, it prints out the the lines that contains the whole word in addition to the file that contains it.

The -w is useful because it allows us to see the lines that contain the string.

[Source](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## -i

-i is used to ignore cases for matching. This means that the string that is trying to be found is not gonna be case-specific, meaning that it'll show the string both lower-case and upper-case.

### Example 1

    bdikbas@Buraks-MacBook-Pro written_2 % grep -i "lucayans" */*/*.txt
    travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
    travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

### Example 2

    bdikbas@Buraks-MacBook-Pro written_2 % grep -i "The Bahamas are" */*/*.txt
    travel_guides/berlitz2/Bahamas-WhatToDo.txt:Diving and snorkeling. Opportunities for diving and snorkeling in the Bahamas are almost unrivaled in terms of both the quality of the experience and the variety of stunning habitats. The area’s clear waters and numerous coral reefs and rocky outcrops offer an ideal environment for hundreds of species of fish, as well as turtles, dolphins, and, yes, sharks. A number of dive centers offer transport to the sites along with the assistance of experienced and qualified dive masters. The two main centers on Nassau and Grand Bahama are Nassau Scuba Centre (Tel. 362-1964; fax 362-1198; US Tel. (954) 462-3400; US fax (954) 462-4100; website <http://www.nassau-scuba-centre.com,)> and UNEXSO (Tel. 373-1244; fax 373-8956; US Tel. (954) 351-9889; US fax (954) 351-9740). Both of these companies also run trips to Andros, Eleuthera, and Exuma. You’ll also find diving and snorkeling opportunities on the main islands of New Providence and Grand Bahama. And there are special places around the Out Islands that offer exceptional experiences, though not much lively entertainment out of the water. Here is a list of particularly exciting sites:
    travel_guides/berlitz2/Bahamas-WhatToDo.txt:Sailing. With hundreds of unpopulated islands and dozens of empty beaches surrounded by dozens of shallow channels and sounds the Bahamas are paradise for sailors. Safe harbors with superb facilities, cozy coves for a night alone, and the possibility of making short hops to a different port every night allow sailors to experience all the different atmospheres of the various islands.

The first command is used to find the .txt files that contain the string "lucayans". When the command is ran, it prints out the the lines that contains the whole word in addition to the file that contains it.

The second command is used to find the .txt files that contain the string "The Bahamas are". When the command is ran, it prints out the the lines that contains the whole word in addition to the file that contains it.

The -i is useful because it allows us to see the lines that contain the string without it being case-sensitive.

[Source](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## > (file name)

In the command line, you're able to put the results of a file into a grep command to organize everything.

### Example 1

    bdikbas@Buraks-MacBook-Pro written_2 % grep -l "Lucayans" */*/*.txt > grep-results.txt
    bdikbas@Buraks-MacBook-Pro written_2 % cat grep-results.txt 
    travel_guides/berlitz2/Bahamas-History.txt

### Example 2

    bdikbas@Buraks-MacBook-Pro written_2 % grep -w "Lucayans" */*/*.txt > grep1-results.txt
    bdikbas@Buraks-MacBook-Pro written_2 % cat grep1-results.txt 
    travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
    travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

The first command is used to find the .txt files that contain the string "lucayans". When the command is ran, it puts the results into a file called grep-results.txt. Then, the newly created file is printed with the cat command in order to show the results.

The second command is used to find the .txt files that contain the string "Lucayans" and is used to match the entire word. When the command is ran, it puts the results into a file called grep1-results.txt. Then, the newly created file is printed with the cat command in order to show the results.

The > is useful because it allows us to organize all the information that we get from the grep command into a file.

[Source](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
