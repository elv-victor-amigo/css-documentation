# Styling Customization of Eluvio Live Marketplace

Once a tenancy is created and the marketplace object is minted, the tenant admin must set the 'theme' of the marketplace to custom. This will allow them to customize their marketplace's CSS directly on the fabric browser by simply setting the desired values to specific root variables. In order to avoid any issues in terms of styling, we highly recommend customizing your site by solely changing the values of the following root variables instead of trying to override any styling with custom stylesheets. 

## Root Variabales
  
  - BACKGROUND: change site's main background color. Primary sets header, filter and stats background colors. Secondary provides a different row shade to Activity table 

        --color-page-bg
        --color-bg-primary
        --color-bg-secondary
  

  - FONT: import your desired fonts using CSS format. Primary used for headers, tertiary used for buttons and secondary for all the rest.

        --font-family-primary                  /* Primary font should be accompanied with 'text-transform: uppercase' */
        --font-family-secondary
        --font-family-tertiary
        --font-default
        
  - FONT COLOR: set color of site's text. Primary changes main text (headers, titles, stats, prices). Secondary changes descriptive text. Highlighted text can be changed using either HEX or RGBA color system. 

        --color-text-primary
        --color-text-secondary

        --color-text-highlight
        --color-text-highlight-rgb

  --color-loader: rgba(255, 255, 255, 0.5);

  --border: 1px solid #444444;
  --border-faint: 1px solid #333333;


  --border-color: #444444;
  --border-color-faint: #333333;

  --box-shadow: none;
