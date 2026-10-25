# Advanced Edge Computing lecture library

Open `index.html` to browse all 11 lectures. Search by topic or lecture number, filter completed lectures, and keep a study checklist in your browser. No build tools or dependencies are needed.

## Host on GitHub Pages

1. Create a GitHub repository.
2. Upload `index.html` and the entire `pages/` folder into the root of the repository. Keep the folder structure and lecture filenames unchanged. You can also upload this README.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the branch containing your files (usually `main`) and **/ (root)**, then save.
6. Once deployment finishes, open the website link shown on the Pages settings screen.

Links are relative, so the library works under a repository's GitHub Pages path as well as when opened locally. Search and checklist features run entirely in the browser. Progress is specific to the browser and site address; it does not sync across devices or between local and hosted copies.

## Add another lecture

Put the new lecture HTML file in `pages/` and add another `<article class="card">` in `index.html`, following an existing card. Give it a unique `data-number`, a lowercase `data-search`, and the correct relative link starting with `pages/`. Update the displayed lecture totals and the progress element's `max` attribute to match.

## Folder structure

- index.html: searchable lecture library
- pages/: all lecture HTML files
- README.md: setup and hosting instructions
