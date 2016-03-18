# Project data/DB mapping
 
## High level structure 
 
Information is organized in a hierarchy of DiscourseParts of different types 
 
* Discourse: a bunch of projects in the same software ecosystem 
  * DiscoursePart: GITHUB_OWNER A person or organization that owns 
    * DiscoursePart: GITHUB_REPO A repository representing a project or subproject 
      * DiscoursePart: GITHUB_ISSUE 
        * Contribution: ISSUE_HEAD The description of an issue, and each item in a comment thread under it 
      * DiscoursePart: GITHUB_PULL_REQUEST 
        * Contribution: PR_HEAD The description of a pull request, and each item in a comment thread under it 
        * Contribution: COMMIT The description text of a commit. 
      * DiscoursePart: GITHUB_PUSH 
        * Contribution: COMMIT The description text of a commit. 
      * DiscoursePart: WEBSITE An information website possibly with multiple pages 
        * Contribution: WEBPAGE A webpage associated with a project 
          * Content: WEBPAGE The text of a webpage, in plaintext, with html and javascript junk stripped out 
            * Annotation: HYPERLINK Ranges of text that refer to other pages 
          * DataSource: URL of the page 
 
## Github Issues and Pull requests 


```python
if x=4:
    happens(3)
else:
    happens(4)
```

You should buy:
- [x] eggs
- [ ] milk
- [ ] pork rinds
- :smiley: :frown:


  
THis is a :smile: smiley face :angry:

Now I'm going to make some references to the 171st issue in scisoft-net map:
- First by pasting the URL directly: https://github.com/cbogart/scisoft-net-map/issues/71
- URL without the s in https follows: http://github.com/cbogart/scisoft-net-map/issues/71
- Then by using just the number: #71
- Then by repo + number: scisoft-net-map#71
- Then by user + number: cbogart#71
- Then user + repo + number: cbogart/scisoft-net-map#71
- Then I'll try a url but substitute PR for issue: https://github.com/cbogart/scisoft-net-map/pull/71

Experiment 2: Usernames:
- My username preceded by at sign: @cbogart
- My github home page url: https://github.com/cbogart
