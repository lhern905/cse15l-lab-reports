# Lab Report 3 - Bugs & Commands

## Par 1- Bugs
```
  @Test
  public void testReverseInPlace2(){
    int[] input = {5, 4, 3, 2, 1};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[] {1, 2, 3, 4, 5}, input);
  }
```

```
  @Test
  public void test2(){
    int[] input = {1,1};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[] {1, 1}, input);
  }
```
![Image](r5_symptm.png)

```
 static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```

```
   static void reverseInPlace(int[] arr) {
     int[] arrClone = arr.clone();
     for(int i = 0; i < arr.length; i += 1) {
       arr[i] = arrClone[arr.length - i - 1];
     }
   }
```

By creating a clone of the originally array we can then iterate and replace the contents of the original array. This fixes the problem that by iterating when we get to the second half of the array it starts to mirror the first half. So now it can reverse the array in the same array with the help of a second array.

##Part 2 -Researching Commands 
Less

-N
```
less -N ./technical/plos/pmed.0020148.txt
      1 
      2   
      3     
      4       
      5         
      6         Cardiovascular diseases (CVDs) are responsible for more than 16 million deaths
      7         worldwide, about 30% of total global deaths. Many of these deaths could be prevented by
      8         tackling major risk factors such as overweight and obesity as a result of unhealthy diet
      9         and physical inactivity, and smoking. Traditionally, CVDs have been considered a “Western”
     10         disease or a “disease of affluence” and not a pressing public health concern for low-income
     11         populations. However, within upper-middle-income and high-income countries, CVDs and their
     12         associated risk factors are increasingly concentrated among the lowest socioeconomic
     13         groups, and globally, 80% of all CVD deaths are in low-income and middle-income
     14         countries.
     15         In this month's 
     16         PLoS Medicine , Majid Ezzati and colleagues conclude that a large
     17         proportion of the world's population living in low-income and middle-income countries
     18         should indeed be the focus of attention for CVD risk factors. This attention is needed
     19         because the aging populations of the currently low-income and middle-income countries are
     20         expected to be those among whom major cardiovascular risk factors will increasingly be
     21         concentrated.
     22         The patterns of risks in relation to one another and to economic variables such as
     23         income are not fully established at the population level but need to be understood if
     24         better long-term policies and interventions are to be deployed. Ezzati and colleagues
     25         examined when interventions should be started by looking at the relationship between
     26         nutritional cardiovascular risk factors—overweight and obesity, and elevated blood pressure
     27         and cholesterol—and three economic indicators, using data for more than 100 countries.
     28         Their analysis uncovered economic–epidemiological patterns more complex than the “Western”
     29         or “affluence” labels would suggest. They found that body mass index (BMI) and cholesterol
     30         increased rapidly in relation to national income, then flattened, and eventually declined.
     31         BMI increased most rapidly until an income of about I$5,000 (international dollars) and
     32         peaked at about I$12,500 for women and I$17,000 for men. Cholesterol showed a similar
     33         pattern, but with some delay. The authors also found an inverse relationship between
     34         BMI/cholesterol and the share of household expenditure put towards food, and a positive
     35         relationship with proportion of population in urban centers, which may be due to changes in
     36         patterns of diet and physical activity with city life. For blood pressure and cholesterol,
     37         possible contributors to the decline at higher levels of income include dietary changes and
     38         use of pharmacological interventions.
     39         As more interventions for blood pressure and cholesterol are adopted in high-income
     40         societies, the three risk factors will become a feature of low-income and middle-income
     41         nations, the authors say. Demographic and technological changes are increasingly modifying
     42         the income patterns of cardiovascular risk factors and shifting their burden to the
     43         developing world; as a result, low-income and middle-income countries will simultaneously
     44         face the burden of infectious disease and cardiovascular risk factors. Unless better
     45         interventions are pursued, we will face a world in which all major diseases are the
     46         diseases of the poor, the authors warn. (See also the Perspective by Thomas Novotny [DOI:
     47         10.1371/journal.pmed.0020104].)
     48       
     49     
     50 
```
```
less -N ./technical/plos/pmed.0020226.txt
      1 
      2   
      3     
      4       
      5         
      6         Richard Smith's key suggestion [1] is that medical journals “should stop publishing
      7         trials” and concentrate on “critically evaluating them.” This bold and radical suggestion
      8         deserves wide debate. It's obvious that many medical journals are losing relevance as
      9         vehicles for scientific information, but it's unclear what will save them. Even as journals
     10         strive to better enforce their conflicts-of-interest disclosure rules, drug companies will
     11         strive to find or create other publication outlets that can communicate to physicians
     12         precisely what advertisers wish to communicate. In sum, an unanticipated effect of purging
     13         clinical trial reports from medical journals might be an even larger proliferation of frank
     14         advertising outlets and messages that might more effectively catch doctors' attentions.
     15       
     16     
     17   
```
The -N command is meant to help you see how many lines are in the text. This is useful for when trying to compare to different files and which one has more lines of text in them. I found this command from this website, [Scaler](https://www.scaler.com/topics/less-command-in-linux/#)

-M
```
less -M ./technical/government/Media/5_Legal_Groups.txt  
ampaign by an alliance of the non-profit providers of free legal
services. "And Justice for All," which solicits donations primarily
from Utah lawyers and foundations, was the first joint fund-raising
campaign of legal services agencies in the country, and the
Community Legal Center is the first joint office project of public
service law groups.
The Legal Aid Society of Salt Lake, the Disability Law Center,
the Multi-Cultural Legal Center, the Senior Lawyer Volunteer
Project and Utah Legal Services will share the new facility, and
last Wednesday their board members were given a tour of the
Community Legal Center hosted by staff members of the five
agencies. All of the agencies can share the same reception area and
client waiting room. The building is close in, across the street
from West High and two blocks from the Gateway. It has its own
parking, something that's hard to find downtown and which has been
a problem for staff as well as clients. Owning and sharing the
building and not paying rent times five will save the non-profit
agencies about $375,000 each year. My assistant, Charity
Christenson, pointed out that the shared facility will also be
efficient for those needing legal services. No longer will a woman
desperate for a protective order, for example, have to run all over
town trying to find the right agency.
After the tour, we found Jaye Olafson at the cookies and
brownies reception on the first floor. Jaye and her husband, Erik,
own Tomax Technologies and were the sellers of the building. Jaye
explained how much of the renovation had been merely uncovering
what was already there. The hardwood floors, wooden ceilings and
brick and stone interior walls were all hidden behind coverings and
old paint. She loves the building, and they only moved out because
the business had outgrown the space. So they renovated the old
Sweet Candy Company building for Tomax. The Olafsons are delighted
with the new owners. The building had been like home, she
explained, and so it was important who would be living there. I
noted on the donor list that the couple, through Olafson Group, had
become one of the major supporters of the project.
Stewart Ralphs, the executive director of the Legal Aid Society,
explained that the Community Legal Center Campaign still has a long
ways to go, with a bit more than half of the $4 million projected
cost received so far. There still needed to be furnishings and
office equipment and such. He promised that they would be getting
in touch with us later on the subject.
./technical/government/Media/5_Legal_Groups.txt lines 16-56/60 100%
```
```
less -M ./technical/biomed/1471-2091-3-8.txt
Background
Thiamine is a water-soluble, B-complex vitamin that
cannot be synthesized by mammals, and thus thiamine can be
obtained only from dietary intake. This can lead to severe
consequences in humans when thiamine is limiting; thiamine
deficiency may result in beriberi and the Wernike-Korsakoff
syndrome [ 1 2 ] . Being positively charged and present in
relatively low plasma concentrations, thiamine movement
across cellular membranes requires transporters. Upon being
taken up by a cell, thiamine is rapidly diphosphorylated by
thiamine diphosphokinase to give thiamine diphosphate
(ThDP) [ 3 ] . Thus, thiamine represents only a few percent
of the total cellular thiamine/thiamine phosphate
derivatives. ThDP serves as a cofactor for several enzymes
that are found both in the cytosol (transketolase) and
mitochondria (α-ketoglutarate dehydrogenase complex being
the most studied example). The intracellular concentration
of ThDP has been estimated at 30 μM, with only about 7
percent being free cytosolic and the remainder being
enzyme-bound with much of this within mitochondria [ 4 5 ]
. Previous findings indicate a complex, cell-type dependent
regulation of compartmentalization and intracellular pools
of thiamine and its phosphorylated derivatives in response
to fluctuating extracellular thiamine levels [ 4 5 6 ] .
Hence, thiamine transport, including that by mitochondria,
is of interest.
Thiamine entry into mammalian cells occurs by a
saturable, high affinity transporter that is deficient in
humans with thiamine-responsive megaloblastic anemia (TRMA)
[ 7 8 9 10 11 12 ] . Thiamine uptake by mitochondria has
been demonstrated [ 13 ] , yet thiamine diphosphokinase is
cytosolic and mitochondria cannot convert thiamine to ThDP
[ 14 15 16 ] . Barile and coworkers demonstrated saturable
uptake of ThDP by rat liver mitochondria characterized by a
./technical/biomed/1471-2091-3-8.txt lines 5-38/430 9%
```
The -M command is meant to help as it puts all of the information of what is currently displayed on the terminal at the bottom, with the sub directory, lines that are currently being shown, how many total lines there are, and how far down you are. This is useful as it helps the user figure out what text file they are looking at as well as how close to the bottom of the text file you are.  I found the information about the -M command through using the `man less` command on the terminal.

-p

```less -p "It"  ./technical/911report/chapter-12.txt```
![Image](-pIt.png)
```less -p "The"  ./technical/biomed/ar387.txt  ```
![Image](pThe.png)

The -p command is meant to help as it takes another input of a string and the terminal will then highlight the string that you input in the text. This is useful as when you are trying to look for a specific sentence or word in the text file, you can use the -p command for this. I found the information about the -p command through using the `man less` command on the terminal.

-e

```
less -e ./technical/biomed/cc2171.txt
Introduction
Each year approximately 750 000 patients in the USA
suffer from sepsis. Treatment for this disease costs $16.7
billion annually [ 1 ] . Despite advances in supportive
intensive care and use of appropriate antibiotics, the
mortality associated with sepsis remains high, especially
among those who develop hemodynamic shock [ 2 3 4 ] . Such
patients frequently progress to multiple organ dysfunction
syndrome, which results in a much higher mortality rate
than among patients who do not develop such complications [
3 5 6 7 ] . This life-threatening syndrome is largely
attributed to the cardiovascular abnormalities associated
with septic shock, requiring supportive therapy (e.g.
mechanical ventilation, fluid resuscitation, and
vasopressors) with volume loading, oxygen delivery, and
regional perfusion [ 8 ] . However, there are still many
controversies regarding choice of fluids [ 9 10 11 12 ] ,
vasopressors [ 13 14 15 ] , hemodynamic end-points for
resuscitation [ 16 17 18 19 20 ] , and monitoring
techniques. Findings from a national survey of intensive
care unit (ICU) utilization showed differences in types of
procedures performed between unit types and hospital sizes
[ 21 ] .
The goals of the present study were to examine
systematically the variations in overall resource use,
therapeutic modality use, and outcome in patients with
severe sepsis across academic medical centers, and to
evaluate relationships between therapeutic modality use and
variation in resource use.
```

```
less -e ./technical/plos/pmed.0020281.txt
 
Whistleblowers serve no function if they cannot tell their stories. The present story of
whistleblowing—as discussed, in part, in 
PLoS Medicine —that involves the pharmaceutical industry, pharmaceutical
 benefit management corporations, the managed care industry, and the political and lobbying
forces that zealously guard their secrets could not have been told without the help of
courageous men and women [1, 2] For that reason, those of us who congregated in Washington,
D.C., on May 15th, 2005, at the invitation and support of the Public Library of Science and
the Government Accountability Project feel particularly humbled and grateful to these two
sponsors. Our convictions could not have been aired were it not for the essential First
Amendment work of responsible journalists, who exemplify the best in investigatory
research.
For me, whistleblowing is not a theoretical exercise. It has a human face and tangible
features. It is the face of children and adults who have been injured or killed by
misrepresented pharmaceuticals; clinical research trial results that have been sequestered
from the scientific community and whose incomplete findings cause injury; and
pharmaceuticals that are detailed to physicians, not to save lives or necessarily improve
the health or welfare of the recipients, but to make money.
In the lonely and, at times, discouraging world of whistleblowing, we whistleblowers are
passionate, and often successful, because our efforts have a different goal than the
corporations and political interests whose operations we occasionally challenge. Our goal
is to tell the truth. That honest effort is the source of any ethical difference we can or
might make. Truth is the basis for the power of a whistleblower, one that can withstand the
assault of unprecedented odds against being heard put forth by that sum of political power,
expediency, and money.
A whistleblower's success depends upon competent and articulate media. The debate to
improve the status quo—be it in pharmaceutical marketing or managed-care decision
making—cannot proceed or flourish without it.
Ralph Waldo Emerson, American essayist and philosopher (1803–1882), commented about
success (I have adapted his comments for all of us who gathered in Washington in mid-May
2005): “To leave the world a bit better, whether by a healthy child, a garden patch or a
redeemed social condition; to know even one life breathed easier because you have lived;
this is to have succeeded [as a whistleblower].”
```

The -e command is helpful as it ends the text output showing in the terminal once you scroll all the way to the bottom to the page. This is useful as it makes it so you don't always have to press q to exit out, making it more efficient for the user to end the text file showing. I found this information about the -e command on this website, [itsfoss](https://itsfoss.com/less-command/)

https://www.scaler.com/topics/less-command-in-linux/#
https://itsfoss.com/less-command/
Man vscode
