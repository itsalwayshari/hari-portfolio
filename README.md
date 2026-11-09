# Hari R. S. — 3D Generalist & Filmmaker Portfolio

Personal portfolio website showcasing 3D art, compositing, motion graphics, animation, and visual storytelling.

## Tech
- Static HTML, CSS, and JavaScript
- No build step or package installation
- Hosted on Netlify

## Deploy on Netlify
Import this repository from Netlify using **Add new site → Import an existing project → GitHub**.
Leave the build command empty and use `.` as the publish directory. The included `netlify.toml` already sets the publish directory.

## Add a project
1. Place project cover images and supported media in `assets/projects/`.
2. Edit the `PROJECTS` list in `index.html` (search for `PROJECTS: add your work`).
3. Set the title, tags, panel colours, cover path, optional video path, year, role, tools, and process steps.
4. Commit and push. Netlify will redeploy automatically once the repository is connected.

## Large video files
GitHub rejects regular Git files larger than 100 MiB. The two original MP4s exceed that limit and are therefore not included in the initial GitHub commit. Keep those videos hosted separately (for example, on a video/CDN host) and update their `video` paths in the project data to the hosted URLs, or configure Git LFS with suitable hosting and bandwidth limits before adding them to the repository.

## Contact form
The contact form is configured for Netlify Forms and currently contains `data-demo="true"`. After the first successful Netlify deploy, configure a form notification to **itsharitheartist@gmail.com**, remove `data-demo="true"` from the `<form id="cf">` element in `index.html`, push the change, and test a submission.
