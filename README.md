# Project Index Generator

This repository contains a collection of web pages stored in the `pages/` directory.

## How it works

The `index.html` file uses JavaScript to fetch the list of projects directly from the GitHub API.

1.  It queries `https://api.github.com/repos/Tyrest/tyrest.github.io/contents/pages`.
2.  It dynamically builds the list of links.
3.  It attempts to fetch the `<title>` of each page to display a nice name.

**Note:** Because this relies on the GitHub API, new pages will only appear in the index **after** you push them to GitHub.

## Directory Structure

-   `pages/`: Contains individual project folders. Each folder should have an `index.html`.
-   `index.html`: The home page that dynamically lists all projects.
