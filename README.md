# Hari R. S. – Portfolio

Static site. index.html plus the assets folder. No build step: push to GitHub and Netlify publishes it.

## Folder map (paths are relative to index.html)
assets/hero/      hero background images (hero-bg.webp)
assets/projects/  project cover images (ukki.webp, detour-society.webp, bluewhale-granite.webp, maverick-ai.webp)
assets/video/     showreel.mp4, showreel-720p.mp4, poster.webp
File names are case sensitive and must not contain spaces.

## Hero background (both layers)
In index.html search for "ASSETS". Two lines control the hero:
- heroLight: image behind "HARI R. S." (light layer)
- heroDark: image behind "3D Generalist, Compositor, Film maker" (dark layer shown while dragging)
Use the same file for both, or two different files. Upload the image to assets/hero/ and change the file name.

## Project covers
In index.html search for "PROJECTS: add your work". Change cover:'assets/projects/xxx.webp' in each project line. Fill in title, role, tools and youtube too.

## Showreel
Upload to assets/video/. In the ASSETS block change reel, reelMobile and reelPoster if the names differ.
Make the video start fast (index at the front): ffmpeg -i input.mp4 -c copy -movflags +faststart showreel.mp4

## Contact form
Netlify Forms. After the first deploy, add an email notification to your Gmail in the Netlify dashboard (Forms area). Then remove data-demo="true" from the <form id="cf"> tag if it is still there.
