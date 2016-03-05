---
layout: page
title: Assignment 2 - Due 2016-04-10
permalink: /assignment-2/
---

# Managing Healthcare Data #

As you read in McConigle, there is a continuum as we move from data to
information to knowledge to wisdom.  With the incorporation of computers and
informatics, we need to be able to manage this continuum in such a way that they
can be shared.  Otherwise, the data / information / knowledge / wisdom are trapped
within a single clinical information system (CIS) or within a single
organization.  This is essentially the "interoperability" problem that we hear
about so much these days.

While interoperability is usually framed in the context of sharing data between
organizations or between electronic health records, the problem exists at
multiple levels:

1. Clinicians from different departments within a single medical center may not
be able to effectively share data due to different information systems,
protocols/policies, and even terminology/vernacular.
2. Within a single organization such as Sutter Health or Kaiser, there are many
different deployments/instances of an information system (e.g. EHR) with
customizations and modifications that make interoperability difficult.
3. Given the structure of the healthcare industry, there is often an incentive
to prevent the sharing of data even if it were technologically possible.

The solution is a combination of data standards and data management approaches
that generally allow informaticists to:

1. Manage the transition of data to information to knowledge to wisdom
2. Share data/information/knowledge/wisdom between information systems and
   organizations.

Much of our discussion will revolve around the technology behind data management
and interoperability but keep in mind that the solution will likely include
changes in bureaucracy, policies, and other socio-political issues.

### Grading ###

This assignment is worth 10 points or 10% of your overall class grade.

### Due Date ###

Friday, April 10, 11:59:59 PM

***Late assignments will not be accepted.***

### Reading ###

McConigle, pp. 135-137 (previously assigned in [Assignment 1](/assignment-1/))

Lim et al., Chapter 1 - Computational Knowledge and Ontology - [PDF available
here](/pdfs/Ontologies.pdf)

Benson, Chapter 2 - Why Interoperability is Hard - [PDF available
here](/pdfs/Interoperability.pdf)

Cimino, Desiderata - [PDF available here](/pdfs/Cimino-Desiderata.pdf)

### Lab ###

For this assignment, you will be working both individually and as a team.

First, as a group, choose a domain topic for which you have previously or would
like to implement some sort of clinical decision support tool.  This CDS tool
can be any type of decision support whether it's to help decrease length of stay
or readmissions, to assist at the bedside, or to help with any other clinical
decision-making.  The key requirements are that the CDS tool uses existing data
from a clinical information system as input.  The CIS can be any system ranging
from an hospital-wide EHR to a department specific system.  Ideally, this CDS
tool is one with which everyone on your team is familiar.

Second, individually, create a basic terminology/ontology for the above domain.
Initially, create a list of terms and concepts that represent the data that your
CDS tool requires.  For example, if creating a bedside arrhythmia detection
tool, you would want to add those terms/concepts that capture specific data your
CDS tool would need.  For example, the existence of certain prior diagnoses
within the patient's medical history may lead the CDS tool to determine that a
particular rhythm is a false positive, thus ignoring it.

- Specific cardiac medications (e.g. Digoxin)
- Specific cardiac diagnoses (e.g. congestive heart failure)
- Arrhythmias (e.g. V-Fib, SVT, etc.)

Third, reconvene as a team and compare and discuss your various lists:

- Which concepts occurred in more than one list?
  - Did you use the same terms/words/acronyms?  For example, did someone write
    down "myocardial infarction" vs. "MI" vs. "heart attack"?
- Which concepts only occurred on one person's list?
  - For those who included it, why?
  - For those who did not include it, why?
    - Oversight?
    - Low prevalence/significance?

Fourth, take all of your lists, determine which concepts are the same,
similar, or directly related to one another:

- For those that are the same, the mappings are simple - you essentially have a
  list of synonyms
- For those that are similar, you will need to create mappings between the terms
  - Are the terms similar enough that there is a one-to-one mapping?  In other
    words, you can use them interchangeably and the effect on any downstream
    analytics is negligible.
  - Is one term a super set of the other?  For example, "myocardial infarction"
    and "cardiac diseases" are related such that MI's are a subset of cardiac
    diseases

Last, discuss among your team members your experience in mapping the terms:

- What difficulties did you encounter?
- Did you find the need to discuss any details of the terms/concepts during the
  mapping phase?
- Did this exercise influence your perspective on how to capture, store, or
  manage healthcare data?

**Deliverables**

For this lab, you may submit your lab in any format - outlines, paragraphs,
diagrams, etc. as a PDF uploaded to Canvas.

During the intensive, we will share and discuss your deliverables between the
groups.  Please do not discuss or share between groups.  I find it very
interesting to see the many different approaches people take when trying to
capture knowledge and expertise that has been developed over years of training
and practice.
