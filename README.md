# Alaska Region Annotated Glossary of Data Management Terms

---


## About the Glossary
The terms within the glossary may have different meanings depending upon the context or discipline in which they are used. The Alaska Region Data Stewardship Team (DST) has compiled the annotated glossary to assist in understanding terms used in relation to data management.

The DST will attempt to use common word definitions as provided by the Merriam-Webster Online Dictionary, however, terms used within technical disciplines, policies or legislation often have definitions that vary from those in common use.

This glossary is intended to help users understand terms that are commonly used within the broader data management community and to identify the preferred use of a particular term within the context of Alaska Region Data Management.

### See also:
* **Merriam-Webster.com dictionary:** (The Government Publishing Office Style Manual. References “Webster’s Third New International Dictionary”; the online version should be similar)

* **Project Open Data**
 
* **Open Government Data Act**: (codification of act definitions: 44 usc 3502)

* **Open Data Handbook Glossary**

* **Glossary of Archival and Records Terminology**: (Society of American Archivists, SAA)

* **Webopedia Computer and Internet Dictionary**


---

## How the Glossary is Set Up

---

### The YAML Config File

A main configuration file titled as "**_config.yml**". This file has the site title and theme within it. 

```yaml
theme: jekyll-theme-leap-day
title: AK Fish & Wildlife Glossary
```

This will apply title and style for the static site. The title can be altered as needed.
Additional information on themes for Jekyll can be found <a href="https://jekyllrb.com/docs/themes/" target="_blank">here</a>. 

---


### The Main Site Page

The homepage is setup on the "**index.md**" file.

This is just a basic home page for the glossary site and can be edited with updates notices
or resource links as needed.

### The Glossary Pages

Each letter in the glossary has it's own markdown file created from A to Z.

The format for a definition entry is show below:

```markdown
### **ADIwg:** 
Alaska Data Integration working group, [ADIWG](https://www.adiwg.org/).
```

- The three # marks provide the H3 heading format for the term. 
- The double asterisks surrounding the term provide the bold format for the term.
- The term's definition is entered on the next space below the term itself.


### Included Navigation

Each page has the same navigation content at the top using an include option. This provides the letter navigation at the top of each glossary page. The file is located within the "**_include**" folder.

```markdown
### **[Go back to home](https://ironrico.github.io/TestGlossary/)**

{% include nav1.html %}
```

### The Expanded Definition Code

Some entries in the glossary are lengthy and have been shortened on the page with the use of a user expansion option. The user can choose to click on the prompt to expand the full definition should they choose to.  
  
The code for using this is shown below.

```markdown
<details>
  <summary>Click to read full definition!</summary>
	<p>
	   The expanded content goes between the paragraph tags
	</p>
</details>
```
- This would be entered after the definition. 
- The text between the "**summary**" tags can be changed if desired.
- The expanded content is placed inside the paragraph tags.

A working example is provided below:

```markdown
### **Archive Folder:** 
A consistent file structure with use constraints and backup schedule.
<details>
  <summary>Click to read full definition!</summary>
<p>
A consistent file structure with use constraints and backup 
schedule that houses the definitive record of a project’s data resources. 
Products in the archive folder are the subject of metadata records and 
are the versions intended for use and dissemination. 
Contrast with working folder.
</p>
</details>
```

---


