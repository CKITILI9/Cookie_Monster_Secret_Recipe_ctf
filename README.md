#Cookie_Monster_Secret_Recipe_ctf
- this challenge teaches us how to inspect website cookies.
---



#Steps Taken
- Launched the picoctf game by clicking on the link.
- the link took me straight to a web page with a username and password field.
- entered a random username and password, and got this clue: 
    Cookie Monster says: 'Me no need password. Me just need cookies!'
    Hint: Have you checked your cookies lately?
- opened developer tools using ctrl+shift+I, to inspect cookies.
- Navigated to the application tab, and saw the cookies to the webpage.
- clicked the http link under cookies and found a base64 encoded text.
- to decode the text, I used echo <'base64 string'> | base64 -d. Where echo means print this string, then decode it (-d)
- decoded the flag and found the flag.
---



#Lessons Learnt
- web apps use cookies to manage data.
- this data is sometimes, not protected.
- analyzing and testing client side data stored in cookies is important.
- base64 encoding is not encryption. the text can be decoded easily.
- base64 is only used to encode and decode binary data into text-based format
---




#Flag
- picoCTF{[REDACTED]}
---




----
