# Stegenography in C

### Created by Matthew Frankland (Feburary 2018)
### Source Code Locked Due to Similarities with Current Coursework. Email mf48@hw.ac.uk to Request Password.

## Problem Specification

To create a cmd program for encoding/decoding PPM3 files in C.

Within my C Program, I implemented three data structures:
    1. A linked-list structure to hold the comments associated with PPM images:
        • My implementation involved creating a node structure and a function to add a node to a singly linked list.
        • I chose to use a single-linked-list in order to store an arbitrary number of comments as I did not have any prior knowledge about how many comments would be in a file. Thus, the program could read each line into the linked list while it started with “#” which denotes a comment.
    2. A structure to hold the rgb (red, green, and blue) values of PPM images:
        • I chose this structure in order to use an array of rgb data within a single PPM image structure. This allowed for easier manipulation of the rgb values, especially in printing the data.
    3. A structure to hold the PPM image data:
        • I encoded message characters using ASCII values so that the integer was always within 255. I calculated the height to put this character value by making a call to a randomiser and take the modulus of this value and the width. This allowed for the value to never be placed outside the size of the PPM.
