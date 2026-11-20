Blogger traffic map package
===========================

Files required in the same folder on your static host:

1. index.html
2. shp_su_intenzity.zip

The HTML automatically loads:
    ./shp_su_intenzity.zip

Do NOT rename the ZIP unless you also change ZIP_URL near the top of index.html.

Recommended hosting: GitHub Pages
---------------------------------
Create a public GitHub repository, upload index.html and shp_su_intenzity.zip,
enable GitHub Pages in Settings > Pages, and choose the main branch / root.

Your published address will look approximately like:
https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/

Blogger embed
-------------
In Blogger, create/edit a Page, switch to HTML view and insert:

<div style="width:100%;height:900px;max-width:100%;overflow:hidden;">
  <iframe
    src="https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/"
    title="Slovakia road traffic intensity 2022"
    width="100%"
    height="900"
    style="border:0;display:block;"
    loading="lazy"
    allowfullscreen>
  </iframe>
</div>

For a taller map, change both 900 values, e.g. 1000 or 1100.

Important
---------
This package does not include the SSC ZIP because the binary file was not
uploaded into the ChatGPT conversation. Add the exact ZIP you already use
successfully with v4:
    shp_su_intenzity.zip
