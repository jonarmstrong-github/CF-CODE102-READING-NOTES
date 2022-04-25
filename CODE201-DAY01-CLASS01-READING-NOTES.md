# CODE FELLOWS - CODE 201

## DAY 01 CLASS 01


### [HOME](README.md)

## AGENDA
1. Introduction to Development
1. Web Site with proper HTML, CSS, JavaScript Structure

## READING
### From the Duckett HTML book:
* Introduction (pp.2-11)
* HTML Chapter 1: “Structure” (pp.12-39)
* HTML Chapter 8: “Extra Markup” (p.176-199)
* HTML Chapter 17: “HTML5 Layout” (pp.428-451)
* HTML Chapter 18: “Process & Design” (pp.452-475)

### From the Duckett JS book:
* Introduction
* JS Chapter 1: “The ABC of Programming” (pp.11-52)

# READING NOTES
## HTML/CSS Chapter 1: “Structure” (pp.12-39)
BLOCK ELEMENTS
> ```<HTML><BODY><H1><P>```

TAGS/ELEMENTS
> ```<ELEMENT>``` Opening Tag

> ```</ELEMENT>``` Closing Tag

ATTRIBUTES PROVIDE ADDITIONAL INFORMATION
> ```<ELEMENT ATTRIBUTE="VALUE">```

HEAD PROVIDES PAGE INFORMATION

> ```<head></head>```
>
> The head contains information not displayed in the browser window.

> ```<title>SHOWN AT THE TOP OF THE BROWSER OR TAB</title>```
>
> The title contains information displayed at the top of the browser window or tab.

## HTML/CSS Chapter 8: “Extra Markup” (p.176-199)

Every HTML element will carry a unique ID attribute.

Class attributes do not need to be unique.

Block elements create a new line for themselves.

```<DIV ID="unique name">```

```<SPAN CLASS="classification">```

## HTML/CSS Chapter 17: “HTML5 Layout” (pp.428-451)

TRADITIONAL HTML LAYOUTS
>```<BODY>```
>
>>```<DIV ID="PAGE">```
>>
>>>```<DIV ID="HEADER">```
>>>
>>>>```<DIV ID="NAV">```
>>
>>>```<DIV ID="CONTENT">```
>>>
>>>>```<DIV CLASS="ARTICLE">```
>>>>
>>>>```<DIV CLASS="ARTICLE">```
>>>>
>>>>```<DIV ID="SIDEBAR">```
>>>
>>>```<DIV ID="FOOTER">```

NEW HTML5 LAYOUTS
>```<BODY>```
>
>>```<DIV ID="PAGE">```
>>
>>>```<HEADER>```
>>>
>>>>```<NAV>```
>>
>>>```<DIV ID="CONTENT">```
>>>
>>>>```<ARTICLE>```
>>>>
>>>>```<ARTICLE>```
>>>>
>>>>```<ASIDE>```
>>>
>>>```<FOOTER>```

"The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure."

HTML5 may be a problem for older browsers.

## HTML/CSS Chapter 18: “Process & Design” (pp.452-475)

WHO IS THE SITE FOR?

THE TARGET AUDIENCE?
- INDIVIDUALS?
- CORPORATIONS?

WHY ARE PEOPLE GOING TO VISIT?

WHAT ARE YOUR VISITORS GOING TO TRY TO ACHIEVE?

WHAT INFORMATION WILL YOUR VISITORS NEED?

HOW OFTEN WILL PEOPLE VISIT YOUR SITE?

START TO ORGANIZE A SITE MAPS TO HELP YOU PLAN.

CREATE A WIREFRAME THAT SHOWS THE HIERARCHY OF INFORMATION AND HOW MUCH SPACE IT MIGHT NEED.

DOES YOUR VISUAL DESIGN HELP YOU COMMUNICATE YOUR MESSAGE?

CREATE A VISUAL HIERARCHY TO HELP DISPLAY INFORMATION.

GROUP TO MAKE DESIGN EASIER TO COMPREHEND.

MAKE NAVIGATION THAT IS CONCISE, CLEAR, AND SELECTIVE.  IT SHOULD PROVIDE CONTEXT, BE INTERACTIVE, AND SHOULD STAY CONSISTENT.

## JAVASCRIPT & JQUERY  Introduction

HTML/CSS REFRESHER
>HTML ELEMENTS GENERALLY HAVE AN OPENING AND CLOSING TAG.
>
>THE ELEMENT MAY ALSO HAVE AN ATTRIBUTE NAME WITH AN ATTRIBUTE VALUE.

>CSS RULES START WITH A SELECTOR AND SOME PROPERTIES IN A DECLARATION BLOCK.
>
>THE DECLARATION BLOCK MAY CONTAIN MULTIPLE PROPERTIES AND THEIR VALUES.


## JAVASCRIPT & JQUERY Chapter 1: “The ABC of Programming” (pp.11-52)

### THE ABCs OF PROGRAMMING

A SCRIPT IS A SERIES OF INSTRUCTIONS

1. WHAT IS YOUR GOAL IN WRITING A SCRIPT?  WHAT IS THE TASK TO ACHIEVE?
1. THE SCRIPT IS A FLOW CHART.
    - BREAK THE GOAL INTO A SERIES OF TASKS.
    - WHAT TASKS DOES THE COMPUTER NEED TO DO?
    - TAKE A PROGRAMMATIC APPROACH.
    - THE COMPUTER WILL FOLLOW INSTRUCTIONS 1 BY 1.
1. THE CODE
    - WRITING EACH STEP FOR THE COMPUTER

SYNTAX - HOW TO ORGANIZE CODE.

### WHERE DO COMPUTER FIT?

CREATE MODELS USING DATA

OBJECTS
> PROPERTIES TELL US ABOUT THE OBJECT.
>
> METHODS (FUNCTIONS) PERFORM TASKS.
>
> EVENTS ARE TRIGGERS FOR THE TASKS.

HTML ELEMENTS ARE LIKE OBJECTS.

### SCRIPT FOR WEBPAGES

HTML - CONTENT LAYER / SEMANTICS

CSS - PRESENTATION LAYER

JAVASCRIPT - BEHAVIOR LAYER

LINKING JS TO HTML CAN EFFECT LOAD TIME

LINKING IS USUALLY DONE AT THE END OF THE BODY BECAUSE OF THIS.

```<SCRIPT SRC="./"></SCRIPT>```

OBJECT
> ```DOCUMENT.WRITE("HELLO WORLD");```
>
> DOCUMENT REPRESENTS THE WHOLE WEBPAGE
>
> . IS CALLED A MEMBER OPERATOR SEPARATING THE OBJECT AND THE METHOD BEING CALLED.
>
> THE METHOD HOLD THE PARAMETERS "HELLO WORLD".
> 

## CLASS NOTES

All labs in 201 will require config files for GitHub.

Scripts go last in the body.

Inline styling wins over all others.

### New Submission Instructions  `(`Copied from Canvas`)`
> Go to https://gist.github.com.
> 
> In the “Gist description…” field, put your name.
> 
> In the “Filename including extension…” field put ‘index.html’.
> 
> Copy-paste your code into the big input field for the Gist.
> 
> Select the button that says “Create secret gist”.
> 
> Choose the “Share” option in the drop down list next to the link.
> 
> Copy the link from the Gist screen for submission in the URL field below.

## LINKS

[www.HTMLANDCSSBOOK.com](https://www.htmlandcssbook.com/)

[Emmet 2.0 in Visual Studio Code](https://code.visualstudio.com/blogs/2017/08/07/emmet-2.0)

## VOCABULARY

Concatenate - the combining of strings

## THINGS I WANT TO KNOW MORE ABOUT

## LEARNING THAT OCCURRED AND PROBLEMS THAT ARE SOLVED

### Emmet
Today I noticed that my Emmet was working the way it worked for others.  I found the link listed above which explained some default settings and allowed me to get Emmet working for me.  Possibly a blessing and a curse.

### Quotes
JavaScript does not care whether you use single or double quotes in strings. This can get very confusing when trying to output variables into quoted text.
> alert('"'+rOne+'!" the kid "' + rTwo + ' yelled out as he jumped into his convertible ' + rThree + " and drove off with his friend's " + rFour +' dachshund."');

### ALL THAT STUFF AT THE TOP OF AN HTML FILE
>```<!DOCTYPE html>```
>
>BE ABLE TO EXPLAIN ANY CODE YOU USE.
>
> ```<html lang="en">```
>
>Sets default language
>
> ```<meta charset="UTF-8">```
>
> UTF-8 is a variable-width character encoding used for electronic communication. Only valid encoding for HTML5.
>
>```<meta http-equiv="X-UA-Compatible" content="IE=edge">```
>
> Defines the pragma directive used to access compiler-specific preprocessor extensions.
> 
> ```<meta name="viewport" content="width=device-width, initial-scale=1.0">```
>
> States that meta data applies to the entire viewport.
> Sets the pixel width of the viewport to the device width.
> 
> ```<title>TITLE</title>```
>
> Defines the document's title that is shown in a browser's title bar or a page's tab.
> 
> ```<link rel="stylesheet" href="css/style.css">```
>
>Applies specific styles


## PROBLEMS THAT HAVE TIMED OUT BEFORE RESOLUTION

### THIS TOOK HOURS.

THE INSTRUCTIONS FOR READING NOTES STATE THAT IT SHOULD ONLY TAKE 15-30 MINUTES TO 'SKIM' A CHAPTER.  THERE WERE SIX CHAPTERS TODAY.  THAT CAME TO 3 HOURS.  TO BE HONEST IT TOOK MORE THAN THAT INCLUDING THE TIME AND EFFORT TO TAKE NOTES AND FORMAT THEM AND THE BREAKS REQUIRED DURING THE PROCESS.  WAS THE 4-5 HOURS OF EFFORT THIS TOOK REALIZED?  INTENDED?

### GitHub config files
~~In class we were told there were files that we would have to download and start putting into our repositories.  I am not entirely sure I was supposed to do this today as we did not create any new repositories but could not find the files.~~

[201 Configs](https://github.com/codefellows/seattle-code-201d85/tree/main/configs)

### [HOME](README.md)