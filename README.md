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
                
                
### Text color and background
        
   * Text color
                
                text-primary
                text-secondary
                text-info
                text-warning
                text-success
                text-danger
                text-light
                text-dark
                text-white
                
   * Background color
                
                bg-primary
                bg-secondary
                bg-info
                bg-warning
                bg-success
                bg-danger
                bg-light
                bg-dark
                bg-white
                
 ### Spacing
   
   Formula: 
                {kind of spacing} {position} - {0-5}
            
                kind of spacing : m or p (margin or padding)
                position        : t,b,l,r,x,y and nothing.
                0-5             : 0 being less to 5 being more.
   
   * Margin (**m**)
        
                mb-0    : margin bottom 0
                mb-1    : margin bottom small amount
                .
                .
                mb-5
          
          similarly
                
                mt-0    : margin top
                ml-0    : margin left
                mr-0    : margin right
                
                mx-0    : margin left and right 
                my-2    : margin top and bottom 
                
                m-5     : margin all sides
                
   *  Padding (**p**)
            
            Same as margin.
                pb-0
                
   
   * Center align
                
                mx-auto
   
   
### Sizing
   
  * width (**w**) and height (**h**)
  
        formula:
            sizing-percentage
    
       sizing | percentage %
       -------|-----------
       w or h | 25,50,75,100
       ---------------------
        
            ex: w-25
                h-50
  
 ### Border
        
   Formula:  border {border-bcolor} {border-{position}-0}
            
        border  : for light border
        
        For border with color:
            Add border-(bootstrap-color-class)

        Ex: border border-danger
            border border-success
            
            
        To remove border on some side
            border border-info border-bottom-0
   
   
   
 ## Buttons
    * Normal buttons
    
          btn : to make a bootstrap styled button
          Pair it with btn- {primary to dark} for different shades.
          EX: btn btn-primary
            btn btn-info
            
    * Ouline buttons        
              
           btn-outline-{primary to dark}
    
    * Link
            
            btn btn-link
        
    * Button sizes
            
            btn-sm
            btn-md
            btn-lg
    
    * Button states
            
            active
            disabled
            toggle : And a data-toggle = "button" attribute for this to work.
            
            
    * Dropdown
            
            <div class="dropdown">
                <button class="btn btn-primary dropdown-toggle" type="button" data-toggle="dropdown">
                        My Dropdown
                 </button>
                <div class="dropdown-menu">
                    <a class="dropdown-item" href="#">Link One</a>
                    <a class="dropdown-item" href="#">Link Two</a>
                    <a class="dropdown-item" href="#">Link Three</a>
                </div>
            </div>
    
    * Split dropdown
            
            <div class="btn-group">
                <button class="btn btn-primary" type="button">My Button</button>
                <button class="btn btn-primary dropdown-toggle" data-toggle="dropdown" type="button">
                    <span >Toggle Dropdown</span>
                </button>
                <div class="dropdown-menu">
                    <a class="dropdown-item" href="#">Link One</a>
                    <a class="dropdown-item" href="#">Link Two</a>
                    <a class="dropdown-item" href="#">Link Three</a>
                    <div class="dropdown-divider"></div>
                    <a class="dropdown-item" href="#">Link Four</a>
                </div>
            </div>
    
    * Button group
        
            <div class="btn-group">
                <button class="btn btn-info" type="button">Left</button>
                <button class="btn btn-success" type="button">Middle</button>
                <button class="btn btn-warning" type="button">Right</button>
            </div>
        
    * Button toolbar
    
            <div class="btn-toolbar">
                <div class="btn-group mr-3">
                    <button class="btn btn-warning" type="button">1</button>
                    <button class="btn btn-warning" type="button">2</button>
                    <button class="btn btn-warning" type="button">3</button>
                    <button class="btn btn-warning" type="button">4</button>
                </div>
                <div class="btn-group mr-3">
                    <button class="btn btn-warning" type="button">5</button>
                    <button class="btn btn-warning" type="button">6</button>
                    <button class="btn btn-warning" type="button">7</button>
                </div>
                <div class="btn-group mr-3">
                    <button class="btn btn-danger" type="button">8</button>
                </div>
            </div>

    * Button vertical group
                
            <div class="btn-group-vertical">
                <button class="btn btn-warning" type="button">Left</button>
                <button class="btn btn-white" type="button">Middle</button>
                <button class="btn btn-success" type="button">Right</button>
            </div>
