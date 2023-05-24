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

#### Example2: 
Command: ```grep -n "While" technical/911report/chapter-10.txt```.    
Output: ```11:            While the plan at the elementary school had been to return to Washington, by the time
409:                Clarke recalls the President telling them." See if he's linked in any way." While he believed the details of Clarke's account to be```. 

```grep -n``` is to find the given words, display the lines and line number in a spacific file. It's useful because we can easily find out that the word we want in the exactly which line and line numbers of a file. 

### For ```grep -o``` : 
-o : is used to extract only the matched patterns or substrings from the input text.
Here are the two examples: 
#### Example1: 
Command: ```grep -o "composing" technical/911report/chapter-11.txt``` 
Output: ```composing```

#### Example2: 
Command: ```grep -o "people" technical/911report/chapter-13.1.txt```
Output: ```people
           people
           people
           people
           people
           people
           people
           people
           people
           people
           people
           people```
                                                                                
```grep -o``` is dispays the same times of the given words. It is useful for various text processing tasks since it allows us to extract specific patterns or substrings from a file or input stream.         


### For ```grep -c``` : 
-c : count the number of lines that match a specified pattern in a file or input stream.
Here are two examples: 
#### Example1: 
Command: ```grep -c "WAR" technical/911report/chapter-2.txt```.    
Output: ```2```                               

#### Example2: 
Command: ```grep -c "public" technical/911report/chapter-6.txt``` 
Output: ```12```                                               

                                                        
```grep -c``` displays the count of matching lines instead of the actual lines themselves. It's useful because it allows us to quickly determine the number of lines that match a particular pattern in a file or input stream.     


### For ```grep -r``` : 
-r : is used to recursively search for a pattern in files within a directory and its subdirectories. It scans all files and directories within the specified directory, searching for occurrences of the specified pattern. 
Here are two examples: 
#### Example1: 
Command: ```grep -r "CONFIGURATION" technical/``` 
Output: ```technical//government/About_LSC/CONFIG_STANDARDS.txt:STATE PLANNING CONFIGURATION STANDARDS Final Task Force Report
technical//government/About_LSC/CONFIG_STANDARDS.txt:STATE PLANNING CONFIGURATION STANDARDS
technical//government/About_LSC/State_Planning_Special_Report.txt:STATE PLANNING & RECONFIGURATION
technical//government/About_LSC/State_Planning_Special_Report.txt:II. LSC CONVENES RECONFIGURATION TASK FORCE
technical//government/About_LSC/State_Planning_Special_Report.txt:IV. REPORT ON LSC'S RECONFIGURATION STANDARDS
technical//government/About_LSC/State_Planning_Special_Report.txt:V. RECONFIGURATION REVIEW PROCESS```

#### Example2: 
Command: ```grep -r "MCDONOUGH" technical/``` 
Output: ```technical//government/Media/5_Legal_Groups.txt:BY EDWARD MCDONOUGH```

```grep -r``` is useful because it allows us to perform a recursive search for a pattern in multiple files within a directory and its subdirectories, making it convenient for searching through large codebases or directories with nested files.

The definition of four grep are from grep --help;
