# css-helper

## Custom CSS Selectors Helper

[Link](https://www.youtube.com/watch?v=VYIDZ57mMy4)

>CSS selector Faster as compare to XPath
B’cz XPath Travers from top to bottom inside DOM, 
Where CSS directly hitting that particulate node

Reference or Practice [DemoSite](  https://app.hubspot.com/login)

1. ID : htmltag # id , #id 

		 input#username, #username 

2. Classname : htmltag . Classname, .classname, c1.c2.c3, htmltag.c1.c2.c3…cn 

	   .form-control.private-form__control.login-email 

3. Parent node > Child Tag

		  div.private-form__input-wrapper>input#username 

4. htmltagname[id=‘value’] 

		 input[id='username']  

		 in Xpath //div[@id=“value”]

  > with one more property — css with 2 attribute 

    div[id=‘value’][type=‘abc’] - css input[id='username'][type='email'] 
    
    //div[@id=‘value’ and @type=‘abc’] 

5. Contains in css  

    	 input[id*=‘user’] or input[id*=‘name’] 

6. Starting Text: 

   		   input[id^=‘user’] 

7. Ending Text:  
    
		 input[id$=‘name’] 

8. Comma in CSS

    	   htmltag.classname, htmltagname#id  

9. First-of-type  

    	 ul#id>li:first-of-type — out of all the list take first element 

10. Last-of-type

    	   ul#id>li:last-of-type — out of all the list take last element 

11. Nth-of-type — specific index  

    	 ul#id>li:nth-of-type(5) - go to 5th in list  

    	 ul#id>li:nth-of-type(n) - it will collect all the li’s - select all —elements 

12. Sibling of element  

	htmltag.classname+htmltagname  

   		 div.classname+div.classname - - select the next element

	 	 div.private-form__input-wrapper+div.private-form__meta 

13. Not operator in css

      htmltag.classname1.classname2:not(.classname3) - - it will exclude classname3  

    .form-control.private-form__control:not(.login-email)

