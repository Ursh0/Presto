# Presto

Presto is a lightweight web-based presentation builder inspired by slides.com.  
It allows users to create, edit, and present interactive slide decks directly in the browser.

The application is built with React and communicates with a RESTful backend API.

---

## Features

### Authentication
- Landing page with login and registration options  
- User registration with validation (password confirmation)  
- Login with error handling  
- Logout available on all authenticated pages  

---

### Dashboard and Presentations
- Dashboard showing all user presentations  
- Create new presentations with:
  - Title  
  - Description  
  - Thumbnail  
- Presentation cards display:
  - Name  
  - Thumbnail (or placeholder)  
  - Description  
  - Number of slides  
- Click a presentation to open the editor  
- Delete presentations with confirmation prompt  

---

### Slide Management
- Each presentation starts with one slide  
- Create new slides (added to the end of the deck)  
- Delete slides (cannot delete the final remaining slide)  
- Navigate slides using:
  - On-screen arrows  
  - Left and right keyboard keys  
- Disabled navigation at first/last slide  
- Slide number visible in bottom-left corner  
- Slide number reflected in the URL for deep-linking and refresh persistence  

---

### Slide Elements

Slides support multiple element types:

#### Text Blocks
- Custom width and height (percentage-based)  
- Editable content  
- Font size in em  
- Hex colour input  
- Left-aligned text  
- Soft border visible in editor  
- Editable via double click  

#### Images
- Size configuration  
- Upload from local file (base64 encoded) or URL  
- Alt text support  
- Editable via double click  

#### Videos
- YouTube embed support  
- Size configuration  
- Autoplay toggle  
- Editable via double click  

---

### Element Interaction
- Elements appear in top-left when created  
- Elements respect layering order (newest on top)  
- Right click deletes an element  
- Elements can be repositioned by dragging  
- Elements can be resized using corner handles  
- Elements cannot overflow outside the slide boundaries  
- Minimum size enforced  

---

### Styling and Themes
- Global font selection for text elements  
- Slide background options:
  - Solid colour  
  - Gradient  
  - Image background  
- Default background applied to new slides  
- Individual slides can override background  

---

### Presentation Preview
- Preview mode opens in a new browser tab  
- Fullscreen slide view  
- Navigation arrows still functional  
- Slide numbers visible  
- No editor borders or controls shown  

---

### Additional Functionality
- Slide transition animations between slides  
- Slide reordering via drag-and-drop interface  
- Revision history with restore functionality  
- Fully responsive layout  
- UI feedback uses components (no alert popups)  

---

## Testing
- Component tests written using Vitest  
- UI tests simulate real user behaviour  
- Tests cover key flows such as:
  - Registering  
  - Creating a presentation  
  - Editing content  
  - Navigating slides  
  - Deleting presentations  
  - Logging out and back in  

---

## Linting
- ESLint configured  
- No warnings or errors when running:
  ```bash
  npm run lint
# Presto
