# Quickstart-Docu-Mayerhofen
Quickstart documentation for Project Mayerhofen

NOTE - the official "Getting started" is now handled at the SUSE Technical Reference Documentation

       Document:
       https://documentation.suse.com/trd/linux/single-html/linux_gs_slessap_fortinet_azure_landscape-automation/

Source:
       https://github.com/SUSE/technical-reference-documentation/tree/main/linux/start/fortinet 

# Assumption(s)
- Most of the text-based content is in AsciiDoc ( https://github.com/asciidoc/asciidoc ) format
- To create any number of multiple output formats, install and leverage DAPS ( https://github.com/openSUSE/daps )

# Usage / Process
- either git clone/fork or download a ZIP (and then unzip) of this GitHub repository
- in the top-level directory, review/adjust/modify the following files:
  - [DC-...]: It is the build file for DAPS, you can  add/enable/disable any of the attributes/sections that you desire
  - [adoc]) : Is the main directory for the documents
  - [images]) : Provides the images for the documents to be used in DAPS
-  To create an output document
  - daps -d DC-SA format
    - where format might be "pdf", "html", "html --single" and many others are also available
  - and example is at create_pdf.sh 
- you can also add images/media content as needed in those subdirectories

- The resulting document will be in the [build] subdirectory

# Feedback
- feel free to provide feedback, ask questions or even submit pull request
