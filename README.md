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

## config.json

Defines app-wide URLs, Game Categories and images and action urls for the home view Features' carousel

Example: 

```
{
    "feedbackURL": "https://move38.com/pages/blinks-support",
    "signupURL": "https://move38.com/sign-up",
    "storeURL": "https://move38.com/collections",
    "supportURL": "https://move38.com/pages/blinks-support",
    "categories":
    [
        {
            "identifier": "popular",
            "name": "Most Popular",
            "featuredGameIds": []
        },
        {
            "identifier": "new",
            "name": "Newest",
            "featuredGameIds": ["crownfall", "bomb-brigade", "berry", "alchematch"]
        },
        {
            "identifier": "exclusive",
            "name": "App Exclusives",
            "featuredGameIds": ["alchematch", "bomb-brigade"]
        },
        {
            "identifier": "all",
            "name": "All Games",
            "featuredGameIds": ["alchematch", "berry"]
        }
    ],
    "featuredProducts":
    [
        {
            "imageURL": "https://app.move38.com/blinks/features/sakura-hero.png",
            "url": "https://move38.com/collections/coming-soon/products/blinks-sakura-strategy-pack"
        },
        {
            "imageURL": "https://app.move38.com/blinks/features/puzzle-wizard-hero.png",
            "url": "https://move38.com/collections/coming-soon/products/blinks-puzzle-wizard-pack"
        },
        {
            "imageURL": "https://app.move38.com/blinks/features/coming-soon-hero.png",
            "url": "https://move38.com/"
        }
    ]
}
```

- `category.featuredGameIds`: Games that should appear in the category on the Shop landing view. The app makes no attempt to verify that the game actually belongs to the category. If empty, the category will not appear on the Shop landing view

## Details HTML

It is important that the body and first and last elements have 0px top and bottom margins so that the iOS client can correctly calculate the height of the html content.