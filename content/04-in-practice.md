---
layout: default
title: Metadata in Practice
nav_order: 4
---
# Metadata in practice

It is good practice to structure metadata using standardized schemas, standards, and formats created and maintained by research communities.

>“In order to be useful, metadata needs to be standardized. This includes agreeing on language, spelling, date format, etc.” ([UNC Metadata for Data Management](https://guides.lib.unc.edu/metadata/standards))

Getting the metadata schema and standards within set-up at the beginning of the project is very important in ensuring future usability. You should also consider the type of resources you’re creating, and what can be understood from them (or not).
* If a textual resource has all the information on it (e.g. names, dates, etc.), the metadata may be able to be created by the repository from the resources.
* If the content is non-textual (e.g. images, multimedia, datasets), not in the language of the repository, etc. there's not much the repository can do to create that metadata, and as a result the content may not be usable or cannot be accepted.

Sometimes it makes sense to create free text “readme” style metadata. In the research context, readme files are often used to document information before being transferred to a more standardized format, or if no appropriate standard exists. It also provides instructions and context to understand and use resources such as datasets.

Metadata can be generated as part of an automated process, or be created manually. Research projects often involve a mix of both, depending on the content and destined platforms for deposit.

It’s highly recommended that at the beginning of your research project, you think about where your research will be stored and made accessible. If it’s destined for something like a repository, there are considerations that should be taken in both content and metadata creation. The purpose of the research can help determine what metadata is necessary for understanding and reproducibility.

## Metadata schemas and standards
What are metadata schemas and standards? Communities create, manage, and use different types of information and resources in different ways. Within and across communities, there needs to be some consistency in order for the metadata to be understandable (by both people and machines) ([University of Texas Libraries](https://guides.lib.utexas.edu/metadata-basics/standards)).

A metadata schema establishes a common way of structuring the metadata, and includes a list of elements (fields) that describe the resources.
* Elements could be Title, Identifier, Creator name(s), Date(s), etc.

Standards provide guidance in how to populate elements within a schema.
* What pieces of information goes where?  
* How should the information be formatted (e.g. dates, names)?
* Are there standardized terms (e.g. controlled vocabulary, thesauri) that should be used to populate an element?

Schemas used for databases or projects often adapt one or more schemas and/or standards, and then create a custom schema based on those.

Custom elements can be necessary to meet the needs of the project, though one must understand that it may not be able to translate in that way in another platform/system (e.g. repository deposit).
{: .note}

There are many types of metadata schemas, varying in audience, complexity, and specificity (disciplinary vs. interdisciplinary). Generic schemas may be easier to use and thus more widely adopted, but can lack coverage for specific types of information. Some disciplines have established metadata standards with specific vocabulary and structure to meet the needs of that research area. In addition, some data repositories have their own schema and standards.

Some common schemas and their disciplines include (but are not limited to):

--------|-------------
Dublin Core (DC) | Interdisciplinary (general, basic, and widely used)
DataCite | Used for for creating DOIs (unique identifiers)
Data Documentation Initiative (DDI) | Social, behavioral, and economic sciences
Darwin Core (DwC) | Biological sciences
ISO 19115 | International standard for geospatial information
MAchine-Readable Cataloging (MARC) | Bibliographic and authority information
Text Encoding Initiative (TEI) | Machine readable creative and interpretive representation of texts or manuscripts
Music Encoding Initative (MEI) | Machine readable representation of music

Dublin Core example ([cIRcle @ UBC Library](http://hdl.handle.net/2429/76411))

<img src="content/images/DCmetadata_01.png" alt="cIRcle DC example 1" width="510"/>

<img src="content/images/DCmetadata_02.png" alt="cIRcle DC example 2" width="510"/>

* Here’s a screenshot from cIRcle (UBC’s digital repository), which uses Dublin Core (these screenshots are from the back-end repository platform so you can see the schema elements, but presents a bit differently publicly). It uses the Dublin Core schema with selected elements (some of which are repeatable, some of which use controlled vocabulary). The elements are flexible for the variety of content held by the repository, and the schema has a flat structure.


DDI example ([ICPSR](https://www.openicpsr.org/openicpsr/project/116562/version/V1/view;jsessionid=507E1914F18B7353C7EE776D4B248030))

<img src="content/images/DDImetadata.png" alt="DDI example" width="510"/>

* Here’s a screenshot from the Inter-university Consortium for Political and Social Research (ICPSR), which is a data archive for the social sciences. It uses the DDI schema, expressed here in XML. You can see it’s a bit more complex with hierarchies and element attributes.

ISO 19115 example ([U.S. Geological Survey](https://www.sciencebase.gov/catalog/file/get/59f8af92e4b063d5d309f043?name=USGS_BBLEH_2012.xml&allowOpen=true))

<img src="content/images/ISO19115metadata.png" alt="ISO 19115 example" width="510"/>

* Here’s a screenshot from the U.S. Geological Survey. It uses ISO 19115, also expressed here in XML, and you can see it’s hierarchical as well. There are relationships between the elements that become apparent when you see how they are nested. Additionally, some elements can be repeated in different contexts.

## More on metadata schemas and standards

As we’ve seen with some examples, metadata schemas can be flat (e.g. Dublin Core) or more complex with hierarchies and repeatable fields (e.g. ISO 19115). This standardized metadata is typically stored in file formats like xml, json, csv. There are also software tools that can be used to create metadata that adheres to a given standard, or express it in a given file format.

Many databases and platforms allow for metadata export in other schemas and formats, which facilitate interoperability and sharing. So standardization is very important to permit this compatibility.
* Crosswalking is the process of translating elements from one metadata schema to another. This facilitates and allows interoperability and harvesting across multiple platforms and systems, increasing research discovery and use. For example, crosswalking metadata facilitates record harvest from Canadian repositories to Canada’s [Federated Research Data Repository (FRDR)](https://www.frdr-dfdr.ca).

## Which metadata schema is right for my project or resource?

Schema can vary in their complexity:

<table>
<tr>
<th>Benefits of basic standards (e.g. Dublin Core; DataCite)</th>
<th>Benefits of complex standards (e.g. DDI; ISO 19115)</th>
</tr>
<tr>
<td>
* Accessible and easy to interpret
* Interoperable - it can be applied to a wide range of resources and used in a wide range of settings
* Easy and quick metadata creation
</td>
<td>
* Comprehensive description
* Potentially for increased discoverability
* Specific to subject area
</td>
</tr>
</table>

Generally, you should be able to find a metadata schema that suits your research. Discuss with colleagues in your research area or those who are doing similar work; they may be able to guide you to preferred standards (and share any lessons learned). Keep the user’s perspective in mind - it should make sense for your intended users.

Having a metadata schema with standards set-up at the beginning of the project, agreement on those standards, and known responsibility/accountability in the project team is very important. You should take into consideration what the end goals of the project are. Certain kinds of metadata analysis and manipulation will require metadata to be input in a standardized way. Consistent entry at an appropriate level of detail for varying uses is important.

## More on metadata in practice
It’s important to consider the *accuracy*, *completeness*, *consistency*, and *interoperability* of your metadata, all of which will affect its future discovery and use.

If you’re planning to deposit your research to a UBC Library repository, it’s highly recommended you connect with the unit at the beginning of your project, so we can provide guidance in schema, standards, and preparing your research for submission.

* [UBC Dataverse](https://dataverse.scholarsportal.info/dataverse/ubc): UBC’s research data repository for UBC faculty, students and staff.
* [cIRcle, UBC’s digital repository](http://circle.ubc.ca/): UBC's open access digital repository for published and unpublished material created by the UBC community and its partners.

Other units at the Library may be consulted, depending on the needs and nature of the project.

## Resources
* [Digital Curation Centre (DCC)’s list of metadata standards](https://www.dcc.ac.uk/guidance/standards/metadata)
* [RDA Metadata Standards Directory Working Group (includes descriptions, implementation tools, and use cases)](http://rd-alliance.github.io/metadata-directory/)
* [Seeing Standards: A Visualization of the Metadata Universe](http://jennriley.com/metadatamap/seeingstandards.pdf)
