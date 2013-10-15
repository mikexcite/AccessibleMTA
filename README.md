AccessibleMTA
=============

A project to make New York City Subway apps accessbile to the blind and visually impaired who use screenreders. The goal is to 1) first create a library of regular expressions for changing words that screenreaders typically do not read corree cted and 2) create a libary of simple code files for different platforms for apps developed to navigate the New York City subway. 

This project has three main parts:

1. Wiki: [Substitution Word List](https://github.com/mikexcite/AccessibleMTA/wiki/Screenreader-Accessibility---MTA-Subway---Word-Substitution-List)
2. Wiki: Substitution Regular Expressions
3. Code: Platform-specific code files (above)

### Why this is necessary

A screenreader is a part of a smartphone (or computer) used by the blind or visually impaired that will read out text on the screen when touched or tapped. It is done by machine, and can make significant mistakes. 

The MTA uses many abbreviations, and these can confuse the screenreaders. This is especially true because the MTA does not use periods following most abbreviations, for longstanding stylistic reasons.  

For example, the iPhone's VoiceOver screenreader can guess read "St" correctly when preceded by a number, so in "125 St" the "St" is correctly pronounced "Street" (though at this point it still will say "one hundred twenty-five street", not "one hundred twenty-fifth street"). But in "Rector St" or "Canal St" will be pronounced "Rector Saint" and "Canal Saint". "For 45, 53 and 59 Sts" will be read "For forty-five, fifty-three and fifty-nine S-T-S", and so on. 

Fortunately, the literal "screenreader" is just the default; most modern platforms allow the programmer to modify the text before it is read out. 
