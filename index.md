#Invitation to comment on a proposal for a cohesive research software citation-enabling platform
by Laura Norén\*

\*This overview was written by an ethnographer who has been involved in the astronomy community in the interest of presenting a relatively unbiased summary.

##Overview: Why (and how) to do research software citations in astrophysics well

A group of roughly forty professionals in the astronomy community from university faculty, telescope facilities, grant making foundations, software repositories, journal editors, and libraries met in May 2015 to formulate the goals and establish a plan to build protocols to weave software citation practices into science-as-usual in astronomy.

This effort dovetails with a larger trend in astronomy (and the natural and social sciences) towards more computationally intensive research. Writing research software is becoming an integral part of science-as-usual though norms and protocols for recognizing, sharing, and rewarding those who contribute well-crafted software to the scientific process have not kept pace. As yet, practices for citing, archiving, assessing the quality of, and otherwise integrating software development into the astronomical research processes have been led by forward-thinking voluntarism in a well-intentioned, time intensive, flexible fashion that has produced a set of experts within astronomy who have a clear understanding of the challenges associated with widening research processes to efficiently and sustainably incorporate research software. Voluntary project-based efforts inevitably run into financial and temporal limits. The current meetings aim to establish processes that use human curation wisely (and sparingly) in conjunction with greater automation, some crowd-sourcing, and author-performed tasks.

One of the first questions that arose at the meeting was about what it means to have a contemporary career in astronomical research and what software skills mean for career paths in astronomy. Should tenure decisions take software citations into account? If so, what is the best way to develop well-understood norms for the proper citation of software? Should there be full-time non-faculty positions created in academia for software developers? What about astronomers who spend time working for telescopes, especially as post-docs (or the equivalent)? How can they maintain coherent curricula vitae so that they may be eligible for academic positions in the future? Should software citations mean the same thing as other types of citations? Will papers that cite “too many” pieces of software be respected in the profession? And how many software citations are too many?

The anxiety around this line of questioning is palpable, and not just in astronomy.

At the workshop in May, the group opted to table the career path discussion in favor of addressing a problem that could be solved:  improving the process for citing research software.

Questions about the normative value of software citations is beyond the purview of this effort, though it is clear that changing the technical system around research software will have an impact on the social value of software creation, sharing, citation and archiving. The goal was to make a plan, assign tasks, avoid intractable questions, engage the community who could not attend the event, and solve research software citation.

##Invitation to participate

Please discuss the following proposal here and on social media using the hashtag #astroware (astronomy + software = astroware).

The main purpose of this document is to generate discussion and elicit feedback.

What is the purpose of the proposal for research software citation?
To create protocols, policies, and links between existing platforms for astronomical software citation, sharing, and archiving that are:  
- uniform;  
- public;  
- uninterested in centralized gatekeeper systems;
- using health checks rather than upvotes to indicate value;
- resilient to the (mis)fortunes of specific companies, institutions, and individuals;
- as simple and efficient as Wordpress;
- as useful as git for version control and GitHub for collaboration;
- as robust as the taxonomy and metadata management systems for print publishing;
- as meaningful to peer participation and career progression as journal publishing has been;
- intrinsically incentivized to encourage researchers to upload software in robust ways (e.g. not to their own webpages);
- thinking more about building a better future than carefully archiving the past.

As one of the publishers at the workshop summarized, our strategy is to, "make clear how to [cite and store software] but not require it. Show off success stories and serve the community rather than police the community." This preceded a similar opt-in sentiment adopted by a different group of forty professionals in scientific publishing who released Transparency and Open Publishing (TOP) Guidelines in July. This astroware proposal would help meet TOP Guidelines but is a proposal to build and connect existing platforms and is not a competing set of guidelines.

##To-do list
Please weigh in on the specific tasks below using the numbers associated with each task.
Additional information about working partners is included after the to-do list.

###1. Establish a preferred location for the generation of unique identifiers for software
One goal from the workshop is to select and promote a single place for the generation of unique digital identifiers (DOIs). The criteria for selecting a registry include being able to work with the astronomy community, to establish an appropriate set of metadata collection practices, to automate certain processes, and to allow for manual data collection/correction. Evidence of effective past interactions and high adoption rates is key.

_Zenodo is the proposed candidate to generate unique software-object identifiers._


###2. Define a metadata protocol for software

A major task along the way to registering software and meaningfully sharing it is establishing a metadata schema. The easier it is for researchers to request a registered ID for their software, the more likely they are to do so. Thus, some fields can be automatically populated with no human intervention required, assuming the software repository is within the ecosystem (e.g. GitHub, Zenodo).

Some librarians and academic astronomers voiced a desire to ensure the metadata protocol could integrate with reference tools like EndNote, RefWorks, etc. though no representatives of those companies were present.

The proposed format for metadata is to carry it in a `package.json` type file.

The fields marked with an asterisk are required. All others are optional.

Proposed Metadata schema
```
*Item Type: Software
*Author(s):
	affiliations
Contributor(s):
	Affiliations
*Title:
*One liner description
Description that can be longer than one line (Could this automatically include text from a readme.txt file, if one exists?)
Tags (auto-populated with an option to manually finesse)
Class (e.g. library, utility, simulation, analysis, executable, GUI,…)
*Subject Area (librarians in the group wanted this to be a required field)
Algorithms, Methods
URL to Home Page
DOI to Software (or software metadata, but that would be self-referential)
Primary Citation (to paper or website describing software, if any)
Preferred citation (could be to a repo, paper, website or other item cite-able now or in the future)
Language(s) (e.g. python, javascript not English, Spanish, etc.)
Platform(s) (e.g. Windows XP, Mac OS X, Linux)
Major dependencies
*Version (e.g. 10.x, 12-Jan-2015)
Date of First Release (ideally, this is automatically pulled with an option to manually adjust)
Date of Last Revision (Last Commit) (ideally, this can be automatically pulled in)
Contains / Is a part of/ other relationships
Format for Data Input (MIME type(s))
Format for Data Output (MIME type(s))
Free or fee?
Source of funding
*License
Open Source? (via license type in search interface)
Size in Lines of code OR bytes for compiled code
Typical execution time (e.g. n sec on hardware-spec)
```

###3. Consider normative standards for citing software

Figuring out what needs to be cited in order to maintain the professional norms of the community is closely related to the creation of technical platforms and protocols. This process of arriving at normative behaviors is iterative and emergent. We invite comments around norms but are not currently tackling the project of enforcing behavioral change.


###4. Quarterly workshops

Coordination is the key to successful integration of the existing astronomical research software citation components.

Quarterly technical workshops between publishers, librarians, software developers, telescopic institutions, grant makers, ethnographers, and academic astronomers to see process through development, testing, and implementation are part of the grant currently being proposed.


###5. Who will be involved? Existing keepers of astronomical research software
The demand for a more robust, long-term sustainable process for citing software is a response to both the success and limitations of the current sociotechnical systems for citing, sharing, storing, and discovering software for research. Representatives from all of the organizations mentioned below were in attendance at the workshop and have remained actively involved in the efforts to build better sociotechnical systems for sharing astronomical research software. Their insights and willingness to volunteer their time are a phenomenally promising aspect of the current effort.

####Astrophysics Source Code Library

The Astrophysics Source Code Library (ASCL) currently serves the astrophysics community as a free source code registry. Hundreds of volunteer hours of human curatorial labor have gone into the creation of the ASCL. Lessons learned by the human curators point to the necessity to keep some human curation, but incorporate automation and author-based tasks to make sure human time is used efficiently.

####Astrophysics Data System

Any identifier is only as useful as its adoption rate. In this case adoption requires users to request a registry ID and for publishers, libraries, and commercial repositories to recognize registry IDs. Within astronomy and physics, the Astrophysics Data System (ADS) hosted at Harvard and supported jointly by the Smithsonian Astrophysical Observatory and the National Aeronautics and Space Administration (NASA) operates as a digital library and already, “provides access and pointers to a wealth of external resources, including electronic articles available from publisher's websites, astronomical object information, data catalogs and data sets hosted by external archives.” Our goal is to make new protocols that weave neatly together with ADS and ASCL so that past projects are not lost.

####GitHub
Citing software is a primary goal that for many researchers is closely related to the secondary goal of effectively sharing software within the research community. GitHub is currently the most frequently used web-based storage, version control, and sharing repository for astronomical software. Because of GitHub’s dual purpose as a repository and an incubator for ongoing software projects, integrating object identifiers with GitHub-based discovery processes is important for traction. Researchers who are better able to make their software projects discoverable to relevant colleagues are probably more likely to register their own projects.

There is some anxiety about incorporating a for-profit company into the scholarly ecosystem. The reliance of scholarly careers on for-profit academic publishers has generated criticism and frustration in the past. However, GitHub relies primarily on the private sector outside of academia for revenue. When researchers opt to make their repositories open to the public on GitHub, they do not incur fees. GitHub only charges for private storage. Because a sizable number of their private-sector clients pay for storage, GitHub’s revenue growth is healthy without requiring financial input from the astronomy community.

####Zenodo

Zenodo already provides an easy way to “share the long tail of small research results” within the sharing pipelines familiar to astronomers by archiving a snapshot of their software and assigning the snapshot a DOI when a release is made in GitHub. With their group of developers, Zenodo is  taking an active role in the technological development of new protocols and connections between the databases underlying journals, digital ID registries, GitHub, citation software (e.g. Zotero), and other software platforms in the ecosystem.

####American Astronomical Society

Journal publishers like the American Astronomical Society (AAS), which is also the main professional organization for astronomy, are critical partners in any ecosystem of information sharing. Leaders from the AAS were in attendance at the workshop and continue to take the lead in this effort. Separate citation accounting for papers that are about software (“software papers”) and for citations of software within research papers is a logical need. The AAS journals will not only sort these accounting matters, they will also play a key role in drawing the connections between the aforementioned platforms and organizations.


###Concluding: Thoughts on the future of software citation in astronomy

The meeting concluded with a round table (well, actually, there was no table and people were mostly sitting on couches) summing up the perspectives that should drive work forward. A telescopic instrument manager reminded us that, "it is important to get the sociology of this right. It has to be perceived as by developers, for developers. We want to present this as a goodie rather than a process." One of the grant makers invited the group to draft a proposal that would, "[get] the community to participate" because "the essential part is not seeing how the world ought to be but seeing how to get there."

Sharing the proceedings of the workshop and the draft protocols with the broader astronomy community is our good faith effort to be earnestly transparent and to eagerly engage those who were not at the workshop.

###Are you in the astronomical community? Please join the conversation using #astroware
If you think what you have read will solve problems for you, please let us know what kind of work you do with software in astronomy.

If you are coming from another field, feel free to chime in as an ally and share how this proposal could solve problems in your field. Or maybe your field already solved software citation and you want to share some best practices. Please do.

If you think we have missed something, tell us how you would expand.

If you think we have gotten something wrong, kindly share your critique.

Please comment here or use hashtag #astroware if you end up having the 
conversation elsewhere on social media.

# Related projects

- [DueCredit](http://duecredit.org) -- automated collation of references for a given analysis pipeline, including possibly references to "educational materials" or examples of specific methods usage.  Currently Python-scentric but the idea is to support as many environments/platforms as possible in the due course of the project.

# Contributions

You can suggest revisions to this document on GitHub [here](https://github.com/astronomy-software-index/2015-workshop/edit/gh-pages/index.md).
