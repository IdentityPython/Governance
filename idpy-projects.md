Title: Adding and Removing Software Projects to IDPY

DRACC: 0024

Category: Regulatory

Scope: Programme

Authors: Flanagan, H.

Date: DRAFT - February 2021

Canonical copy available at <https://dracc.commonsconservancy.org/0025/>

Copyright: This document is copyright: The Commons Conservancy and IdentityPython. It can be used under a Creative Commons Attribution 4.0 International license.

# Project addition

## Proposal format
Code base maintainers who are interested in having their project brought under the IdentityPython collection should send a message to the discuss@idpy.org mailing list using the following template:

* Introduction of the maintainer(s)
	* Introduction could be just a hello from the person in charge. and a minimal message on that person’s availability in relation to the project development. We do not collect projects, we want the people that develop those to keep doing that and have them become part of the organisation and their project part of the ecosystem.
* Project goals & future
	* Project goals are in direct relation to the project’s future. Their relation with idpy.org goals are the first thing to make sure is aligned.
* How it relates to idpy.org
	* Is there another project that is using the new one as a dependency or enhancement?
	* Is there a relation to a more generic AAI concept?
* Current project state
	* How far is the project from its goals? What are the problems it is facing (technical / community / dedication-time)?
* What other projects does this codebase depend on (if any)?

* Project metadata:
	* URL to project website
	* URL to project source code
	* URL to project ticketing-system (issue tracker)
	* URL to project license
	* Communication channels (mailing-list, slack, irc, etc)

While all these might seem like too much bureaucracy, each of these sections could be a couple of lines or even mangled together in a couple of paragraphs.

Once we have such a proposal we should evaluate the project and come to a conclusion.

## Technical quality

Projects under the IdentityPython banner should include and support the following to allow for easier alignment and administration:

* projects should include documentation posted on readthedocs.io
* projects should follow semantic versioning as described at semver.org
* new releases should include change logs
* projects should include code tests
* projects should add templates for issues and pull requests (see for example <https://github.com/IdentityPython/SATOSA/blob/master/issue_template.md> and <https://github.com/IdentityPython/SATOSA/blob/master/pull_request_template.md>.

## People quality

This is a lot harder to judge, but very important. The community is vital to the organisation’s lifecycle. Growing the organisation means growing the community and accepting more people in its core. While we cannot prevent people from fighting over (many times even non-) technical aspects, we can make a priority to make the community feel safe. Thus we must take notice of how communicative the new project’s maintainers are, what the project’s culture is, and whether this fits to the form of the environment we want to create - an environment where people are polite and try to understand rather than dominate.

This is of course twofold - it is the same thing the other way around. We are dealing with work done by other people. We must respect that and be grateful that they put time in this.

In simpler terms, it is better to not reply to an issue/question/email, if one is irritated, in hurry or stressed. None should feel forced to answer or pressured to keep with others’ pace.

## Organisation stability

While a project may fit perfectly, we should always keep in mind what the organisation’s pace is, and how many things it can process at the same time. Growing should come in a steady fashion to avoid people getting overwhelmed. Enthusiasm is great and needed but should be kept in reason with pragmatism.

There is always a right time to do more. We should not be afraid to reject even good looking matches, as doing so does not mean that there is no way of even having that chance again.

The same way we require a project to be in a certain form to be accepted, the same requirement is on us to be in a state to accept that project.

To put it in another way, the organisation should help its project move forward, and give tools and services to the community. If it is in a state that is struggling, then accepting a new project does not help neither party.

## Discussion and consensus

Everyone should do their homework, go through this list and then decide whether they think it is a good idea and timing to accept the project. While a message outlining their basic reasoning is wanted, a simple +1 or -1 should suffice.

Keep in mind that a “-1” is important to express. It is very common to only see +1 replies, accept the new thing, and then being into a situation where many people do not like the new state but never expressed it. In the long run, this will lead to problems within the organisation.

It is often much harder to express rejection, as it seems to place people in a position where they have to explain themselves. Please consider both +1 and -1 equally important and available with no justification.
Process duration

Individuals will have a chance to express their position for four weeks before a final decision is made.

Needless to say, that the community members must trust the decisions of other members, and as such should not demand that they are present in every process. Rough consensus is what we are striving for - unanimity is pretty hard to achieve.

Once the development community has reached consensus on whether the new project should be included under the IdentityPython banner, the Board will take a final vote and inform the project maintainers as to next steps.

## Aftermath

* Set a member responsible for the overall supervision of the project (the existing maintainer(s) most probably).
* Announce the conclusion to our communication channels (announce-mailing-list, slack, website, blog, twitter, etc.) whatever the conclusion is. Transparency is important for the community as it builds trust and portrays a certain level of maturity.
* Incorporate the code: Add project under the github organisation
* Incorporate the people: Add members to the appropriate lists and other tools (github policies, travis, slack channels etc)
* Open appropriate issues to integrate the new project with existing projects.
* Add to the projects roadmap anything related to the organisation or things that come up in the proposal discussion.

# Project removal

Removing an existing project should follow the same process. The difference is that if decided, the actual process needs planning. The project might be a dependency or part of another project, and as such it should either be replaced (no functionality lost) or removed in way that users and services are not affected.

The same way we want a steady removal of that project, the same thing will be wanted by other people that could be using this. We should reach out to project we know that they are using that component and ask them to either adopt it, or replace it.
