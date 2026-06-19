## Checklist: Cross-Browser and Responsive Testing

## 1. Cross-Browser verification (Chromium and FireFox):
*Goal: Ensure that application logic and layouts work identically across different browsers*

- **Core navigation:** Verify top menu links and dropdowns work correctly in both Chromium and FireFox
- **Session and cookies:** Verify that user login session persists correctly during page reloads in both browsers
- **Form Submissions:** Check that registration, logic and payment forms submit without JS errors in FireFox
- **Media Rendering:** Verify that product images, icons and sliders render properly in both browsers

## 2. Responsive Web-Design and Viewport Testing:
*Goal: Verify that the website layout adapts gracefully to desktop, tablet, and mobile screen resolutions*

### Desktop layout (1920x1080):
- **Full menu visability:** The Header displays the full navigation menu without wrapping into double lines
- **Grid aLignment:** Product items in the catalog are aligned in clean grid

### Table layout (768x1024, Ipad):
- **Adaptive grid:** Product grid scales down gracefully 
- **No horizontal scroll:** The page scrolls only vertically: no elements break out of the screen boundaries 
- **Touch target size:** Buttons and links remain large enough to be easily clickable on a touch screen

### Mobile layout (375x812 Iphone):
- **Hamburger menu:** The main header menu hides behing a "Hamburger" icon (Three lines), and clicking it expands the menu
- **Single column layout:** Product list switches to a single-column layout form easy vertical scroll
- **Cart table adaptation:** The shopping cart table converts into stackable cards or handles horizontal overflow
- **Popups and modals:** "Added to cart" success popups scale down properly and fit within the mobile screen limits


