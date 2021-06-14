# obsidian-snippets

# Table of Contents
- [Dataview Snippets](#Dataview-Snippets)
  - [Across Vault Word Count](#Across-Vault-Word-Count)

## Dataview Snippets

### Across Vault Word Count

<https://github.com/torantine/obsidian-snippets/blob/main/dataviewjs.acrossVaultWordCount-v0.0.11.md>

To function properly, this snippet requires MetaEdit.

A key feature of this snippet is the use of metadata fields, in this case inline dataview fields, as variables inside of dataviewjs. Through the use of MetaEdit and elements, an inline value can be used as a variable that stores its state with the page. Additionally, the dataview table can be exported to inline fields to store the data on the page.



Features:
- Search by tag or modified date
- Output: number of pages, modified date, page links, words, total words, characters, total characters, sentences, total sentences

Known Bugs:
- Upon changing search type to tags, all pages cannot be chosen unless another option is chosen first.

![Across Vault Word Count](https://user-images.githubusercontent.com/52270977/121964956-25fec300-cd21-11eb-96fd-d134958d1bc8.gif)

v 0.0.2 the search term text in target files is no longer counted 
v 0.0.3 fixes non-space-delimited words not being counted. Thanks goes to boniall in the Obsidian discord for pointing out the issue.
v 0.0.4 added `。！？` as defining ends of sentences and `‘ ’ “ ”` as characters able to exist after sentence end
v 0.0.5 an empty tagToSearchFor now returns all files
v 0.0.6 added in modified date column and the ability to export to inline fields
v 0.0.11 added in dropdown menus, search by modified date, export sums to inline fields, dependency check for MetaEdit plugin

## Templater Snippets

Coming Soon...
