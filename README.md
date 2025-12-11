## Retro Banner Site
A single-page personal banner website featuring a nostalgic Windows 95/98 aesthetic. The design uses a fixed-pixel retro frame that scales responsively on all screen sizes using a JavaScript zoom calculation to maintain the pixel-art look.

# Features
Retro UI design with pixelated "Press Start 2P" font.

Fully responsive layout that maintains exact aspect ratios on mobile devices (tested for Galaxy S8+ and similar).

Compact background OR optional Looping video background with a dark overlay for readability.

Functional custom audio player with Play, Pause, Next, and Previous controls.

Typewriter-style blinking cursor animation.

File Structure
For the code to work immediately, ensure your project directory is organized exactly as follows:

Plaintext

/project-folder
|-- index.html
|-- assets/
    |-- frame.png
    |-- pfp2.jpeg
    |-- song1.mp3
    |-- song2.mp3
    |-- song3.mp3
    
# Setup Instructions

Create the Directory: Create a new folder for your project.

HTML File: Save the provided code as index.html inside that folder.

Assets Folder: Create a subfolder named assets.

Media Files: Place your images, background video, and MP3 files inside the assets folder.

Launch: Open index.html in any modern web browser to view the site.

## Customization Guide
# Changing Audio
To update the playlist, scroll to the <script> section at the bottom of index.html. Update the songs array with your specific file paths and display titles:

JavaScript

const songs = [
    { title: "Your Song Title", src: "assets/your-file.mp3" },
    // Add more rows as needed
];
# Changing Images
Frame: Replace assets/frame.png. For best results, keep the original aspect ratio (approx 514x486px).

# Profile Picture
Replace assets/pfp2.jpeg. A square aspect ratio (1:1) is recommended.

# Changing Text
Locate the <div class="text-area"> section in the HTML. You can edit the H1 tag (Name), paragraphs (Status/Loc), and the bio text freely.

# Autoplay
Due to modern browser policies, the audio will not play automatically. The user must click the "PLAY" button to start the music.

Technical Notes
Responsiveness: The site uses a JavaScript function to calculate the available screen width/height and applies a CSS zoom property. This ensures the retro interface does not distort or blur on smaller mobile screens. However, I did run into some issues with the video background implementation and a different background colour may affect your text layout.

## More Info
All songs used in this example are my own songs that I made myself by using FL Studio, feel free to check out my uploads on Bandlab: https://www.bandlab.com/yumewav

