# Custom-Options-For-Monogram

1.) Add jQuery Version js on line no. 9 in theme.liquid before </head> tag.
{{ 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js' | script_tag }}

2.) Add schema code in product-template.liquid at the end of file before {% endschema %} from sections.
	,
	{
		"type":"header",
		"content":"Product Option Personalization"
	},
	{
		"type":"checkbox",
		"label":"Enable on product page",
		"id":"enable_personalization"
	},
	{
		"type":"text",
		"label":"Add Product Tag",
		"id":"product_tag",
		"info":"Display personalization at added above tag exist in product"
	},
	{
		"type":"image_picker",
		"id":"monogram_image",
		"label":"Upload Monogram Image",
		"info":"Upload PNG Image"
	},
	{
		"type":"checkbox",
		"label":"Enable Font Option 1",
		"id":"enable_type_personalization_font_1",
		"default": true
	},
	{
		"type": "font_picker",
		"id": "type_personalization_font_1",
		"label": {
		  "de": "Schriftart 1",
		  "en": "Font 1",
		  "es": "Fuente 1",
		  "fr": "Police 1",
		  "it": "Font 1",
		  "ja": "フォント 1",
		  "pt-BR": "Fonte 1"
		},
		"default": "work_sans_n6"
	},
	{
		"type":"checkbox",
		"label":"Enable Font Option 2",
		"id":"enable_type_personalization_font_2",
		"default": true
	},
	{
		"type": "font_picker",
		"id": "type_personalization_font_2",
		"label": {
		  "de": "Schriftart 2",
		  "en": "Font 2",
		  "es": "Fuente 2",
		  "fr": "Police 2",
		  "it": "Font 2",
		  "ja": "フォント 2",
		  "pt-BR": "Fonte 2"
		},
		"default": "work_sans_n6"
	},
	{
		"type":"checkbox",
		"label":"Enable Font Option 3",
		"id":"enable_type_personalization_font_3",
		"default": true
	},
	{
		"type": "font_picker",
		"id": "type_personalization_font_3",
		"label": {
		  "de": "Schriftart 3",
		  "en": "Font 3",
		  "es": "Fuente 3",
		  "fr": "Police 3",
		  "it": "Font 3",
		  "ja": "フォント 3",
		  "pt-BR": "Fonte 3"
		},
		"default": "work_sans_n6"
	},
	{
		"type":"color",
		"id":"personalization_background_color",
		"label":"Select Background Color",
		"default":"#557b97"
	},
	{
		"type":"color",
		"id":"personalization_heading_text_color",
		"label":"Select Heading Text Color",
		"default":"#ffffff"
	},
	{
		"type":"color",
		"id":"personalization_content_text_color",
		"label":"Select Content Text Color",
		"default":"#000000"
	}
	
3.) Create new snippet as name "personalization" and paste below file code into it.  

4.) Open product-template.liquid from sections and add {% include "personalization" %} before qty box and add to cart button code.

5.) That's it. Now you need to customise and set up settings fonts type from Theme Customise under Product page Tab at Product page sections.

6.) For More details about set up theme customise settings check below screenshots: 

