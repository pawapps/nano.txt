# nano.txt
v0.1.0

Protocol for associating a website with a [Nano Currency](https://nano.org) account

## Getting Started
The nano.txt protocol format is similar to [robots.txt](https://developers.google.com/search/reference/robots_txt) files.  It exists so external entities can find the nano.txt file, understand the contents of the file, and make the appropriate decisions based upon the information in the nano.txt.

When a Nano Currency account is found in a website's nano.txt, it can be assumed that the website owner has control of and can be associated with that Nano Currency account.

## File Path
The nano.txt file shall exist at the root level of a website.

### Examples
- https://example.com/nano.txt
- https://sub.example.com/nano.txt

## Format
Only a single Nano Currency account shall be written on a line.
No other information than Nano Currency account's is in the file

### Examples
The following could be placed at https://nano.org/nano.txt:

    xrb_1ipx847tk8o46pwxt5qjdbncjqcbwcc1rrmqnkztrfjy5k7z4imsrata9est
    xrb_3wm37qz19zhei7nzscjcopbrbnnachs4p1gnwo5oroi3qonw6inwgoeuufdp

## Comments
- Should a label be included with a Nano Currency account?  I think no because a label could be misleading.  A website URL is unique while a label could be used to make someone believe that account, even though on a bogus website, is associated with a known entity.

## Implementation
The following sites/applications are known to utilize the nano.txt protocol (not just have a nano.txt but rely on websites listing their nano.txt):
- https://nanote.io

If you know of an implementation, contact me via [Twitter](https://www.twitter.com/pwlk) or this GitHub, and I will add to the listing.
