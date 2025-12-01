# **How to Transfer Your Styles to Al-Folio**

Once you are happy with the look of the preview above, follow this mapping to apply the changes to your GitHub repository.

## **1\. Changing Colors & Fonts**

**File to Edit:** \_sass/\_variables.scss (or \_sass/\_themes.scss in newer versions).

| Preview CSS Variable | Al-Folio SASS Variable | Example Value |
| :---- | :---- | :---- |
| \--global-theme-color | $theme-color | \#2698ba (Teal) |
| \--global-bg-color | $background-color | \#ffffff |
| \--global-text-color | $text-color | \#2b2b2b |
| \--font-sans | $font-family-sans-serif | "Inter", sans-serif |
| \--font-serif | $font-family-serif | "Merriweather", serif |

**How to change fonts:**

1. Go to \_includes/head.html and paste the Google Fonts link (\<link href="..."\>) from the preview.  
2. Go to \_sass/\_variables.scss and update the font family names.

## **2\. Changing Navigation Style**

**File to Edit:** \_includes/header.html

* **To make the navbar sticky:** Al-folio is sticky by default (fixed-top class).  
* **To change the background blur:** Look for the .navbar class in \_sass/\_layout.scss and add backdrop-filter: blur(5px);.

## **3\. Changing Project Cards**

**File to Edit:** \_projects/ (Markdown files) and \_layouts/page.html (Logic).

* Al-folio defaults to a Masonry grid (tiles fitting together).  
* **To match the Preview's Simple Grid:**  
  * In \_sass/\_projects.scss, you can adjust the .grid-item padding and borders to match the .project-card style in the preview.

## **4\. Custom CSS Overrides (Safest Method)**

Instead of editing theme files, you can usually add a file called assets/css/custom.css (or similar, depending on version) and link it in \_includes/head.html.

**Paste this block to match the Preview's typography:**

/\* Typography Overrides \*/  
body {  
    font-family: 'Merriweather', serif; /\* Or whatever you chose \*/  
}  
h1, h2, h3, h4, nav {  
    font-family: 'Inter', sans-serif;  
}  
a {  
    color: \#2698ba;  
}  
