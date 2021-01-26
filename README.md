## voici un exemple de requête wikidata
'''sparql 
PREFIX bd: <http://www.bigdata.com/rdf#>
PREFIX wikibase: <http://wikiba.se/ontology#>
PREFIX wd: <http://www.wikidata.org/entity/>
PREFIX wdt: <http://www.wikidata.org/prop/direct/>
select distinct ?personneLabel 
where {
?personne wdt:P31 wd:Q5 . #pour chercher des personnes humaines
?personne wdt:P106 wd:Q42973 . #qui occupe la fonction d'architecte
?personne wdt:P27 wd:Q30 . #qui sont américains
SERVICE wikibase:label { 
bd:serviceParam wikibase:language "fr,en"}
}
'''
### Markdown

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Zale-14/WIKIDATA-/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
