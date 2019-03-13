# NAV-Levenshtein-Compare
NAV Levenshtein Compare - Code to handle compare of 2 strings with weighted results

# What’s This??
Imagine the following scenario…. 
You have more than one person in your Org capturing new vendors. Also, everyone has a different way for capturing vendor. Take “Coke n Cola” for example…. One guy Calls it Coke, the next guy calls it “Coke n Cola” and yet a third person fills in the full name as “Coke n Cola Pty (Ltd.)”. You could end up with 3 of the exact same vendors in your system, just named differently. 
This is exactly what the Levenshtein algorithm addresses. If you search on the internet, you will find a plethora of code samples in almost any language imaginable on how to implement this algorithm… Except NAV
# Solution
This is exactly that the code in this repo addresses. It takes to strings as input and returns you a weighted value between 50 and 100 % likelihood of match.
Thus, by looping though the Vendor table and comparing each vendor name to the new vendor name being captured, you will get a likelihood (%) returned of a match. Stack the result in a list ordered by match percentage and you can see if the vendor you are capturing already exists in your system or not.
# Objects
The solution contains only one CodeUnit. With one function exposed that you can call. The OnRun trigger of the CodeUnit contains sample code that you can execute (or copy and paste and execute from anywhere in your system)

# Enjoy
Hope you find this useful. As always if you can make any improvements or found a bug, send me a pull request and ill incorporate it in my code.
