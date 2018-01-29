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
            
   * Outline buttons        
              
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
    
    ```html               
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
    ```

 * Split dropdown
    
    ```html
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
    ```
    
 * Button group
    ```html    
    <div class="btn-group">
        <button class="btn btn-info" type="button">Left</button>
        <button class="btn btn-success" type="button">Middle</button>
        <button class="btn btn-warning" type="button">Right</button>
    </div>
    ```
        
 * Button toolbar
    
    ```html
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
    ```
    
 * Button vertical group
    
    ```html            
    <div class="btn-group-vertical">
        <button class="btn btn-warning" type="button">Left</button>
        <button class="btn btn-white" type="button">Middle</button>
        <button class="btn btn-success" type="button">Right</button>
    </div>
    ```


## List groups
            
                ul will be list-group
                everything under it li/a will be list-group-item
                
                for hoverable list: list-group-item-action
                
                
   * colored list
                
                <ul class="list-group">
                    <li class= "list-group-item list-group-item-primary"> Primary</li>
                </ul>
                
   * tab list
                
                Just like tab window.
                for ex: tablist.html
                
   * badge
                
                badge
                badge-{primary to dark}
   
   * breadcrumb
                
                breadcrumb
                breadcrumb-item
                
                
                
                
 ## Forms
        
        form-group      : to div to group label and input
        form-control    : to input to bootstrap style it
        
  * checkbox:
               
               form-check       : for the div containing label and checkbox
               form-check-label : for checkbox label
               form-check-input : for checkbox input
               
 * Inline form
                
                use form-inline instead of form-group
  
  * Form row
               
               Go readup.
  
  * Validations
                
                is-valid        : for green background around input field
                is-invalid      : for red background
                invalid-feedback: for error messages
                
                Ex:
                        validation.html
                

## Input Groups
            
            Way be merge two input items as one.
            ex: radio button + text field
                text field + (search) button 
                
           Enclosing div is given   : input-group
           And the addon are given  : input-group-addon
           But if its a button      : input-group-btn
           And the text field will have the regular form-control class.
           


## Alerts and Progress bar
               
               alert                    : for enclosing div
               alert-{primary-dark}     : combined with any contextual color
             
             
  * Dismissible alert
                
      ```html
       <div class="alert alert-primary alert-dismissible show fade">
           <button class="close" data-dismiss="alert" type="button">
               <span>&times;</span>
           </button>
           <strong>Dismissable</strong> Blog post added
       </div>
       ```

   * Progress bar
                
                progress        : for enclosing div
                progress-bar    : to render the progress bar
                with bg-{color} for different color progress bars.
                
                progress-bar-striped    : for striped progress bar
                progress-bar-animated   :  to show animation on striped progress bar
                
        example:
        ```html
        <div class="progress">
            <div class="progress-bar progress-bar-striped bg-warning progress-bar-animated" 
                 style="width:80%;"> 80% </div>
        </div>
        ```
    
    
 ## Tables
        
            table           : add table class to table tag to make it bootstrap table
            table-inverse   : reversing the color
            table-striped   : white and grey table
            table-hover     : hoverable table
            table-bordered  : table with border
            table-{size}    : table based on size
            

## Pagination
            
  ```html
  <nav>
        <ul class="pagination">
            <li class="page-item disabled"><a class="page-link" href="#">Previous</a></li>
            <li class="page-item active"><a class="page-link" href="#">1</a></li>
            <li class="page-item"><a class="page-link" href="#">2</a></li>
            <li class="page-item"><a class="page-link" href="#">3</a></li>
            <li class="page-item"><a class="page-link" href="#">Next</a></li>
        </ul>
   </nav>
   ```
              
              to align pagination menu we can use:
                justify-content-start
                justify-content-center
                justify-content-end
                
                
      
 ## Cards
                Read cards.html
            
                    
## Media object 
                
                media
                media-body
                Not so important skim through documentation if you will ever need it.
                

## Grid system
            
            grid.html

## Grid Alignments
        
  * Vertical alignment
                
                align-items-start       : applied to row to align all items to the start
                align-items-center      : to align at the center
                align-items-end         : at the end
                
       * To align individual columns
                
                align-self-start
                align-self-center
                align-self-end
  
 * Horizontal alignments
                
                justify-content-start
                justify-content-center
                justify-content-end
                justify-content-around  : to balance spaces around
                justify-content-between : all empty space will be inbetween
                

## Flexbox
        
        d-flex
        flex-row
        flex-column
        And all grid alignment classes
        
        READ: flexbox.html

   * auto-margins and wrappings
        
                mr-auto
                ml-auto
                mb-auto
                mt-auto
                
                flex-nowrap
                flex-wrap
                
                Ex: autoMargins.html

## Carousel
        Read: carousel.html
        
## Collapse and Accordian
     
   * collapse button
   
                data-toggle     : collapse
                data-target     : div's id
                
                And div should a id and class:  collapse
                
                
   * Accordion
                
               READ accordion.html
