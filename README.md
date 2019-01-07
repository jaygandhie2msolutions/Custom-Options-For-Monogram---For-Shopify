# Custom-Options-For-Monogram

1.) Check jquery js file in your theme.liquid if exists then no need to add it this code else you can add jQuery Version js on line no. 9 in theme.liquid before </head> tag.
{{ 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js' | script_tag }}

2.) Add schema code (schema.liquid) in product-template.liquid at the end of file before {% endschema %} from sections.
	
3.) Create new snippet as name "personalization" and paste below file code into it.  

4.) Open product-template.liquid from sections and add {% include "personalization" %} snippet before qty box and add to cart button code.

5.) That's it. Now you need to customise and set up settings fonts type from Theme Customise under Product page Tab at Product page sections.

6.) For More details about set up theme customise settings check below screenshots: 


### Demo Store:
https://custom-product-option.myshopify.com/products/premium-leather-bag


#### For More Help or Customise as per your custom requirements shoot mail us at shopify@e2msolutions.com or https://www.e2msolutions.com/contact-us

