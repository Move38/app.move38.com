# app.move38.com

### Folder Structure
- /blinks
  - config.json
  - /games
    - games.json
    - /game-title
      - details.html
      - /images
        - rom-art.png
        - header.png
        - image-1.png
        - image-2.png
   - /features
     - feature-image-1.png
     - feature-image-2.png     
- /ios
  - landing page for NFC
- /android
  - landing page for NFC

## Details HTML

It is important that the body and first and last elements have 0px top and bottom margins so that the iOS client can correctly calculate the height of the html content.