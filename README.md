# Boostrap
My Bootstrap journey!


### Basic typography
        
 * Display heading:
        Use to display name of the page for something really big.
        
                display-1   : humongous
                display-2   : smaller than humongous
                display-3   : Biggg
                display-4   : twice h1
 
* Paragraphs:
            
            lead
 
* Style class:
        
        font-weight-bold    : for bold text
        font-weight-normal  : for normal text
        font-italic         : for italicized text
        
 
* Text transform:
        
        text-lowercase  : make text lowercase
        text-uppercase  : make text uppercase
        text-capitalize : ok you got the gist.
        
* List
    
        list-unstyled (for ul)  : to remove the bullet points
        
        list-inline (for ul) and list-inline-item (for li) to make list packed horizontally.



### Text Alignment & Display
        
   * Text alignment (**text**)
        
        Important note: All text alignment classes are prefixed with "text".
        
                text-justify    : to justify a text.
                text-left       : left align text
                text-right      : right align text
                text-center     : center align text

   * Responsive alignment 
        
        All responsive alignments have same class names as regular alignments with size specified in the middle.
                
                text-sm-right   : align text to right on small or larger screens
                text-md-right   : align text to right on medium or larger screens
                text-lg-right   : align text to right on large or larger sreens
                text-xl-right   : align text to right on xl or larger screens
                
                same goes with text-left and text-center.
                
   * Display (**d**)
        
        **d-** followed by the display property.
                
                d-inline        : display as inline element
                d-block         : display as block element
                d-inline-block  : display as inline-blocks.
             

### Floats and Position
        
        float-left      : to move a element to the left
        float-right     : to move a element to the right        
        float-none      : no float
        
   * Responsive floats
                
                float-sm-left
                float-md-left
                
                same pattern
   
   * clearfix
              
              when you float left and float right item say if there is space inbetween 
              them that space will be occupied next immediate markup( a paragaraph or heading tag)
              so avoid that and force a line break we use clearfix.
            
            without clearfix:
              __________                                                   ________
              |previous|         Bootstrap clearfix                        | next |
              ----------                                                    -------
              
             with clearfix: 
              __________                                                   ________
              |previous|                                                   | next |
              ----------                                                    -------
                                                                                                
                                 Bootstrap clearfix                                              
              
              
    * Fixed Top
                
                fixed-top:
                To fix a text at a fixed position irrespective of scrollbar movements use fixed-top class.
    
    * Sticky top
                
                sticky-top:
                To make a text move along with scrollbar once it position is reached.
    
    * Fixed bottom
                
                fixed-bottom
                To fix a text at the bottom of the screen.
