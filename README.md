# BACK Stack Decision Records

This directory contains documents informing the BACK stack's design. BACK stack
designs may transition through up to three of the following phases:

1. Proposals. A proposal is simply a Github issue against this repository with
   the `proposal` label. Proposals need to be at most two
   to three paragraphs.
2. One-pagers. A One-pager is a brief document pitching an idea for further
   experimentation. One-pagers, as the name suggests, are usually around one
   page long. They provide just enough context to achieve buy-in from maintainers.
3. Design documents. A design document is a longer, more detailed design. Design
   documents should typically be preceded by a one-pager and/or a good amount
   of research and experimentation.

All designs start as a proposal. In some simple cases, this proposal alone
is sufficient to proceed with a design. As the complexity or controversy of
the proposed design increases, a one-pager and/or design document may be
required. Please name your documents appropriately when committing to this
repository, i.e. `one-pager-my-cool-design.md` or `design-doc-my-cool-design.md`.

All documents committed to this repository _must_ include the following header:

```markdown
# Document Title
* Owner: Some Person (@GithubUsername)
* Reviewers: Maintainers
* Status: Accepted, revision 1.0
```

The __document owner__ is the person responsible for stewarding its lifecycle.
The owner will typically be the original document author, though ownership may
be handed over to another individual over time. The owner may include
their email address, but it is not mandatory.

The __document reviewers__ are a small, targeted audience. Feedback is _always_
welcome from any member of the community, but feedback from the
elected reviewers carries extra weight.

The __document status__ reflects the lifecycle of the design. Designs may be
If the status is indicated, they are committed to main at any stage in their lifecycle. 

Use one of the following statuses:

* _Speculative_ designs explore an idea without _yet_ explicitly proposing a
  change be made. Typically, only one-pagers will be speculative.
* _Draft_ designs strive toward acceptance. Designs may exist in draft for
  some time as we experiment and learn, but their ultimate goal is to become
  an _accepted_ design.
* _Accepted_ designs reflect the current or impending state of the codebase.
  Documents may transition from _draft_ to _accepted_ only after receiving
  approval from a majority of the document's elected reviewers. Once a
  document reaches _accepted_ status, it should also include a major. The minor
  style abbreviated semantic version number reflects substantial design updates over time.
* _Defunct_ designs are kept for historical reasons but do not reflect the
  current or impending state of the codebase either because they were never
  accepted or because they were accepted but are no longer reflective of the
  state of the codebase.

Note that in some cases designs are "semi defunct". These designs are deemed
relevant enough to keep "accepted" rather than marking them
completely defunct, but may:

* Be only partially implemented.
* Reference defunct concepts.
* Have iterated conceptually, API wise, or code wise since initial
  implementation.

The current convention for such documents is to leave them in the "Accepted"
state, but add a prominent note at the top of the document explaining the way(s)
in which they are no longer accurate.
