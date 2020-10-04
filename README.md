This is for self reflection purpose and to keep track of what I'm doing

### HTML PORTION

1. Add the outline of the page (div,a with links). No css. Just pure HTML.
After adding the the about, store, gmail, images links, I couldn't figure out the little option squares on the top right that shows a collapsed view of Google's services. 
    !!TODO:
    The class of gb_C changes that square picture, if I change it, the image changes to a bell. // Still have to figure this out.  
2. Add the <img> for the profile picture with an <a> parent but it filled up the whole browser
    !!TODO: 
    Use CSS to fit it into the div container
3. The loop in the middle in the search bar is uses a picture as a svg file
    !!TODO:
    Figure out how to add the loop pic
4. Add the search bar and a class 
    !!TODO: 
    Add border, margin, padding 
5. Add a div below the search bar that with two buttons
6. Add two bottom divs with anchor tags 

______

### CSS Curiosities
* `.left-side { position: absolute}`
    Made the left side to align with the right side, note that `.right-side` wasn't positioned. 
* Changing the padding-right of `profile-pic` changed its circular size

---------

Second revision:
Added code  

```
html, body {
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
    overflow-x: hidden; 
}
```
## Header
Google's header has a `div` container for two `div` children, the left and right links each.

1 -> 1a - 1a

### Pending to find out why
While adding style for both `left-header` and `right-header`, again I saw that left used `position: absolute` and right used `position: relative` . 

## Bigger clickable anchor tags
Google's store `a` tag's margi is bigger on the left. Found this when trying to make my anchor tags clickable areas bigger. 

##### What I learned: 
* `position: relative` is useful so that z-index can be used to make the click area stay on top of text that comes next.

## Make the selection outline border non existant

##### What I learned:

It's useful to add `outline: none` to all the document, so making a selector `* {}` in which the outline rule is added. While this solution decreases accessebility in general, I figure it's a better stradegy to maintain the cohesiveness of the general style of the project.