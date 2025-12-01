# **How to Host Your Academic Site on GitHub Pages**

**Recommended Theme: al-folio**

This guide will walk you through setting up your site using **GitHub Pages** and the **al-folio** Jekyll theme. This combination is the "gold standard" for ML and Neuroscience researchers because it automatically handles LaTeX math, Google Scholar citations, and code highlighting.

## **Phase 1: Setup GitHub Repository**

1. **Create a GitHub Account** (if you haven't already).  
2. **Go to the al-folio repository:** [https://github.com/alshedivat/al-folio](https://github.com/alshedivat/al-folio)  
3. **Fork the Repository:**  
   * Click the **"Use this template"** button (green button) or **"Fork"** at the top right.  
   * Name your new repository exactly: yourusername.github.io (Replace yourusername with your actual GitHub handle).  
   * Make sure the repository is **Public**.  
4. **Enable GitHub Actions:**  
   * Go to your new repository's **Settings** tab.  
   * Click **Actions** \> **General** on the left sidebar.  
   * Ensure "Allow all actions and reusable workflows" is selected.  
   * Click **Pages** on the left sidebar.  
   * Under "Build and deployment", set "Source" to **GitHub Actions**.

*At this point, GitHub will automatically start building your site. After about 2-3 minutes, you can visit https://yourusername.github.io and see the default theme.*

## **Phase 2: Configuration (\_config.yml)**

The \_config.yml file is large. **You only need to edit about 10% of it.** Here is exactly what to look for and what to ignore.

### **1\. The "Site Settings" Block (Lines 1-30 approx)**

*Search for title: or scroll to the very top.*

* **Change these:**  
  title: Abdul-Malik Zekri  \# Your browser tab title  
  first\_name: Abdul-Malik  
  last\_name: Zekri  
  email: your-email@usf.edu  
  description: "Researcher in Computational Neuroscience & ML"  
  keywords: neuroscience, machine learning, SNNs, manifolds

* **Ignore these:** lang, unicode, timezone (defaults are fine).

### **2\. The "URL" Block**

*Search for url:*

* **Change these:**  
  url: "\[https://yourusername.github.io\](https://yourusername.github.io)"   
  baseurl: ""  \# Leave empty if your repo is named exactly \`yourusername.github.io\`

  *Note: If you named your repo something else (like my-website), set baseurl: "/my-website".*

### **3\. The "Footer" Block**

*Search for footer\_text:*

* **Change this:**  
  footer\_text: "Powered by \<a href='\[https://jekyllrb.com/\](https://jekyllrb.com/)' target='\_blank'\>Jekyll\</a\> and \<a href='\[https://github.com/alshedivat/al-folio\](https://github.com/alshedivat/al-folio)' target='\_blank'\>al-folio\</a\>."

* **Ignore:** footer\_last\_updated (defaults are fine).

### **4\. The "Social" Block**

*Search for social\_media: or footer\_social:*

* This section enables the icons in the footer/sidebar.  
* **Action:** Uncomment (remove \#) the lines for email, scholar, github, and linkedin. Add your specific usernames.  
* **Example:**  
  github\_username: TheShadowTiki  
  linkedin\_username: abdul-malik-zekri  
  scholar\_userid: YOUR\_ID\_HERE \# Look at your Google Scholar URL for the ID

### **5\. What to IGNORE (Do not touch these)**

* **newsletter:** Leave this section alone or comment it out if you don't want a newsletter.  
* **comments:** (Disqus/Giscus). You don't need comments on a portfolio site.  
* **analytics:** (Google Analytics). You can set this up later if you want to track views, but it's not needed for launch.  
* **cdn:** Leave as default.

## **Phase 3: Migrating Your Content**

The al-folio theme uses specific folders for different types of content. Here is where you paste the text we generated.

### **1\. The Home Page (index.md)**

* **File Location:** index.md (in the root folder).  
* **Action:** Replace the default text with the content from our **HERO SECTION** and **RESEARCH HOOK**.  
* **For News:** The theme has a \_news folder. You can add your "Barry Goldwater" and "CSHL" updates there as individual files, or just write them manually in index.md for simplicity.

### **2\. The Research & Projects (\_projects/)**

* **File Location:** \_projects/ folder.  
* **Action:** Create a markdown file for each of your 4 main projects.  
* **Format:**  
  \---  
  layout: page  
  title: Neuromodulation on Weight Manifolds  
  description: CSHL (Zador Lab)  
  img: assets/img/project\_thumbnail.jpg  
  importance: 1  
  category: research  
  \---

  \*\*Problem:\*\* Standard Reinforcement Learning...  
  (Paste the rest of the project description here)

### **3\. Publications (\_bibliography/papers.bib)**

* **File Location:** \_bibliography/papers.bib.  
* **Action:** This is the best part of al-folio. You don't format the text manually. You paste the BibTeX citation for your papers here.  
* **Example:**  
  @article{walking2025,  
    title={Walking the Weight Manifold...},  
    author={Benjamin, A. and Zekri, A.-M. and others},  
    journal={arXiv preprint},  
    year={2025},  
    pdf={link\_to\_pdf},  
    code={link\_to\_code}  
  }

* The theme will automatically format this into a beautiful list with "PDF" and "Code" buttons.

### **4\. Leadership & About (\_pages/)**

* **Action:** Create two new files in the \_pages/ folder: leadership.md and about.md.  
* **Header:**  
  \---  
  layout: page  
  title: Leadership  
  permalink: /leadership/  
  nav: true  
  nav\_order: 5  
  \---

* **Content:** Paste the respective text for the Leadership and About pages below the header.

## **Phase 4: Customization & Polish**

1. **Navigation Bar:** Open \_data/navigation.yml. Add your new pages (Leadership) to the list so they appear in the top menu.  
2. **Images:** Upload your headshot to assets/img/prof\_pic.jpg.  
3. **CNAME (Optional):** If you buy a domain (e.g., amzekri.com), add a file named CNAME to the root folder containing just your domain name.

## **Need Help?**

If al-folio feels too complex, you can simply **upload the site\_preview.html file** I created for you to a GitHub repository, rename it index.html, and it will work immediately as a single-page website. However, sticking with Jekyll allows for easier updates in the future.