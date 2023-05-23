# Researching Commands

The four interesting command-line options that I chose:   
* grep -n
* grep -o
* grep -c
* grep -r

### For ```grep -n``` : 
-n : is used to display line numbers along with the matching lines of text.
Here are the two examples: 
#### Example1: 
Command: ```grep -n "Although" technical/911report/chapter-1.txt```.                                        
Output: ```266:FAA Awareness. Although the Boston Center air traffic controller realized at an early stage that there was something wrong with American 11, he did not immediately interpret the plane's failure to respond as a sign that it had been hijacked. At 8:14, when the flight failed to heed his instruction to climb to 35,000 feet, the controller repeatedly tried to raise the flight. He reached out to the pilot on the emergency frequency. Though there was no response, he kept trying to contact the aircraft.
402:    In sum, Indianapolis Center never saw Flight 77 turn around. By the time it reappeared in primary radar coverage, controllers had either stopped looking for the aircraft because they thought it had crashed or were looking toward the west. Although the Command Center learned Flight 77 was missing, neither it nor FAA headquarters issued an all points bulletin to surrounding centers to search for primary radar targets. American 77 traveled undetected for 36 minutes on a course heading due east for Washington, D.C.
562:    Inside the National Military Command Center, the deputy director of operations and his assistant began notifying senior Pentagon officials of the incident. At about 9:00, the senior NMCC operations officer reached out to the FAA operations center for information. Although the NMCC was advised of the hijacking of American 11, the scrambling of jets was not discussed.```

#### Examples2: 
Command: ```grep -n "While" technical/911report/chapter-10.txt```.    
Output: ```11:            While the plan at the elementary school had been to return to Washington, by the time
409:                Clarke recalls the President telling them." See if he's linked in any way." While he believed the details of Clarke's account to be```. 

```grep -n``` is to find the given words, display the lines and line number in a spacific file. 
