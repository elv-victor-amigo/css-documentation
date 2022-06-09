# Styling Customization of Eluvio Live Marketplace

Once a tenancy is created and the marketplace object is minted, the tenant admin must set the 'theme' of the marketplace to custom. This will allow them to customize their marketplace's CSS directly on the fabric browser by simply setting the desired values to specific root variables. In order to avoid any issues in terms of styling, we highly recommend customizing your site by solely changing the values of the following root variables instead of trying to override any styling with custom stylesheets.

## Variables

You will be able to make a custom theme with relatively few variable changes since most component variables reference general defaults. The following are the variables that are given custom values and re-used throughout the different components. 
  
  - BACKGROUND: change site's main background color. Primary sets header, filter and stats background colors. Secondary provides a different row shade to Activity table. Add media to your background using the content variable.

        --color-page-bg
        --color-bg-primary
        --color-bg-secondary
        --background-content
        --border-radius-page-content
  

  - FONT: import your desired fonts using CSS format. Primary used for headers, tertiary used for buttons and secondary for all the rest.

        --font-family-primary                  /* Primary font should be accompanied with 'text-transform: uppercase' */
        --font-family-secondary
        --font-family-tertiary
        --font-default
        
  - FONT COLOR: set color of site's text. Primary changes main text (headers, titles, stats, prices). Secondary changes descriptive text. Error sets color of alert messages. Highlighted text can be changed using either HEX or RGBA color system. 

        --color-text-primary
        --color-text-secondary
        --color-text-error

        --color-text-highlight
        --color-text-highlight-rgb
        
  - BORDER: sets border of tables, stats, filters. Faint and highlight variables provide the opportunity to differentiate edges and lines. Use the border parameter variables (radius, color) to fill in the necesary border values. 
        
        --border
        --border-faint
        --border-highlight
        --border-radius
        --border-color
        --border-color-faint
        --border-color-highlight
        
  - CARDS: NFT cards displayed on the marketplace are styled with the below variables. 

        --background-marketplace-card
        --color-marketplace-card-text-primary
        --color-marketplace-card-text-secondary
        --border-marketplace-card
        --border-marketplace-card-logo
        --border-radius-marketplace-card

**The rest of the global variables (listed below) we highly recommend you simply interpolate their values with the ones above. This will decrease the amount of overlapping CSS values and parameters as well as avoid rendering issues.**

  - SITE HEADER

        --font-header-links
        --font-header-profile
        --font-header-balance
        --font-store-header

        --background-page-header
        --color-page-header-text;
        --color-header-link-text
        --color-header-link-text-active

        --background-marketplace-header
        --color-marketplace-header-text
   
  - MARKETPLACE HEADER 

        --font-store-heading
        --font-store-subheading
        --font-store-link
        
  - BUTTONS

        --font-button
        --font-button-selection

        --background-button-primary
        --color-button-primary-text
        --border-button-primary
        --border-radius-button-primary

        --background-button-secondary
        --color-button-secondary-text
        --border-button-secondary
        --border-radius-button-secondary

        --background-button-danger
        --color-button-danger-text
        --border-button-danger
        --border-radius-button-danger
        
        --background-button-selection
        --color-button-selection-text
        --border-button-selection
        --border-radius-button-selection

        --background-button-selection-active
        --color-button-selection-active-text
        --border-button-selection-active
        --border-radius-button-selection-active
        
  - INPUT FIELDS

        --font-input
        
        --background-input
        --color-input-bg-solid
        --color-input-hover-bg
        --color-input-text
        --color-input-text-placeholder
        --color-input-highlight-bg
        --color-input-highlight-text
        --border-input
        --border-radius-input

        --box-shadow-input
        --box-shadow-input-focus
        --outline-input-focus
        
  - LISTINGS AND ITEMS CARDS

        --font-card-title
        --font-card-text
        --font-card-misc

        --background-card
        --color-card-bg
        --color-card-text-primary
        --color-card-text-secondary
        --color-card-text-highlight
        --box-shadow-card

        /* Cards and feature cards have borders implemented as a padded element with a colored background */
        --border-background-card
        --border-width-card
        --border-radius-card

        --color-card-stock-available
        --color-card-stock-unavailable

        --color-card-badge-bg
        --color-card-badge
        --border-radius-card-badge
        
 - FEATURED ITEM CARD

        --font-feature-card-title
        --font-feature-card-text
        --font-feature-card-misc

        --background-feature-card
        --background-feature-card-runway

        --color-feature-card-text-primary
        --color-feature-card-text-secondary
        --color-feature-card-text-highlight
        --box-shadow-feature-card

        --border-background-feature-card
        --border-width-feature-card
        --border-radius-feature-card

        --color-button-feature-card-bg
        --color-button-feature-card-text
        --border-button-feature-card
        --border-radius-button-feature-card

        --border-background-feature-card-selected
        --box-shadow-feature-card-selected

        --color-featured-item-slider
        --color-featured-item-slider-handle
        
 - TABLES

        --font-table-header
        --font-table

        --background-table
        --background-table-header-row
        --color-table-header-row-text
        --color-table-odd-row-bg
        --color-table-odd-row-text
        --color-table-even-row-bg
        --color-table-even-row-text
        --color-table-selected-row-bg
        --color-table-selected-row-text
        --color-table-highlight-text

        --border-table-row-selected

        --border-table-primary
        --border-table-secondary
        --border-radius-table
        --box-shadow-table

        --color-table-badge-active-bg
        --color-table-badge-active-text
        --color-table-badge-inactive-bg
        --color-table-badge-inactive-text
        --border-radius-table-badge
        
 - MODALS

        --background-modal-overlay
        --background-modal-primary
        --border-modal-primary
        --border-modal-secondary
        --border-radius-modal

        --color-button-modal-close-bg
        --color-button-modal-close-text
        --border-button-modal-close
        --border-radius-modal-close
        
 - LOG IN

        --background-login
        --background-login-box
        --color-login-text-primary
        --color-login-text-secondary
        --color-login-text-highlight
        --border-login-box
        --border-radius-login-box
        --box-shadow-login-box
        
  - DETAILS (section boxes, listing stats, etc.)

        --font-component-header
        --font-component-text
        --font-component-misc

        --background-component-primary
        --background-component-secondary
        --color-component-bg-primary
        --color-component-bg-secondary
        --color-component-highlight
        --color-component-text-primary
        --color-component-text-secondary
        --color-component-text-highlight
        --border-component-primary
        --border-component-secondary
        --border-component-highlight
        --border-radius-component
        --box-shadow-component

## Examples

The following are examples of customizations compared to the default CSS of the marketplace.

[Default CSS](https://github.com/eluv-io/elv-media-wallet/blob/main/src/static/stylesheets/themes/default.css#L28) ---> [Site with Default Theme](https://wallet.contentfabric.io/#/marketplace/iq__THqkAiRSaDCRPLtZ81PndCos2zn/store)

[Dark Theme CSS](https://github.com/eluv-io/elv-media-wallet/blob/main/src/static/stylesheets/themes/dark.theme.css) ---> [Site with Dark Theme](https://wallet.contentfabric.io/#/marketplace/iq__38aCx8VAeNFQG2i1ngWS1rfFV6Rx/store)

[Maskverse CSS](https://github.com/eluv-io/elv-media-wallet/blob/main/src/static/stylesheets/themes/maskverse-test.theme.css) ---> [Maskverse Site](https://wallet.contentfabric.io/#/marketplace/iq__2JocoHMZ6YTSWWLf315ibCyMvyFj/store)

[WWE CSS](https://github.com/eluv-io/elv-media-wallet/blob/main/src/static/stylesheets/themes/wwe-test.theme.css) ---> [WWE Moonsault Site](https://www.wwemoonsault.com/marketplace)



