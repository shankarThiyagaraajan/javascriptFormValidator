JavaScript Library For Form Validation
--------------------------------------

#### Why Simple Form Validator ?

1. It's developed by Core JavaScript. 
2. It supports most of browsers.
3. Light Weight Library
4. Very Simple Implementation.
5. PowerFull Form Management. 

**Steps to Integrate to Form :**

``<script src="simpleFormValidator/src/js/formValidator.js"></script>``

Then Integrate your form with Validator.

         <script>
             
             var data = {
             form: 'new_ticket_form',          // Required.
             warning_color: 'aa0000',          // Optional.
             new_class: 'test'                 // Optional.
             };

             // Validation Will Init Here.
             validate(data);
             
          </script>
          
          
Currently the validation will trigger on submit button trigger.

It has automated listener to eliminating unnecessary changes on form.

**Note:**

1. Validation take place between tags, so need to specify the **ID**  
   of the Form or any other tags.
   
           <form id="newUser"> </form>  // Preferred
           
           <div id=newUser> </div>      // Not-Preferred [but it supports]
           
2. Input Fields should specify the type of validation.

           // For Simple Require.
           <input type="text" required name="name">
           
           // For Min Restriction.
           <input type="text" required min=2 name="name">
           
           // For Max Restriction.
           <input type="text" required max=16 name="name">
           
           // For E-Mail Validation.
           <input type="email" required name="name">
           
3. Every Input Fields should have a Label with **FOR** attributes.

           <label for="uname">Name :</label>
           <input type="text" name="uname" required>
           
4. Form Tag Should use **novalidate** to Avoid Browser level validation.
       
           ex. Chrome Browser. 
           
It Will listen the **Submit** button event **Automatically**.

So **No Need** to use ``<input type="submit"..... onClick="validate()" .....>``

###License

MIT License

           
   
