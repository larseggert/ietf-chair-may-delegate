---
title: "The IETF Chair May Delegate"
# abbrev: ""
category: bcp
updates: 9281, 2850, 4949, 8713, 3710
docname: draft-eggert-ietf-chair-may-delegate-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
# number:
# date:
consensus: true
v: 3
# area: ""
workgroup: "IETF"
# keyword:
#  - next generation
#  - unicorn
#  - sparkling distributed ledger
venue:
  group: "IETF"
  type: "Internet Engineering Task Force"
  mail: ""
  arch: ""
  github: "larseggert/ietf-chair-may-delegate"
  latest: "https://larseggert.github.io/ietf-chair-may-delegate/draft-eggert-ietf-chair-may-delegate.html"

author:
-
  name: Lars Eggert
  org: NetApp
  street: Stenbergintie 12 B
  city: Kauniainen
  code: "02700"
  country: FI
  email: lars@eggert.org
  uri: "https://eggert.org/"

normative:

informative:

--- abstract

This document propses that the IETF Chair may delegate some of their
responsibilities to another Area Director. One important aspect of
this is to allow the separation of the IETF Chair and IESG Chair
roles.

--- middle

# Introduction

Throughout the history of the IETF, the role of the IETF Chair has
always been a filled by a single person. None of the foundational
documents of the organization precisely define the role, but most are
written with an understanding that the role is filled by a single
person that is then tasked with with numerous responsibilities. Few
documents explicitly say that the IETF Chair may delegate some of
these responsibilities. Over time, this has created a situation where
even a full-time commitment by a single person may no longer be
sufficient to fulfill all of these roles and duties.

Also, the role of the IETF Chair is a single point of failure for the
organization, with no defined processes for allowing others to
quickly and/or temporarily take over aspects of the role if the IETF
Chair becomes partially or fully unable to serve. (The defined
process is that for "mid-term vacancies" per {{Section 3.5
of !RFC8713}}, which can take up to six weeks to complete and only
allows for the permanent replacement of the IETF Chair by another
individual.)

Single bottlenecks like this have obvious scaling and fault tolerance
issues. This document hence proposes to explicitly allow the IETF
Chair to delegate some of their responsibilities to one or more other
Area Directors. It leaves it up to each IETF Chair to determine if
they would like to delegate some of their responsibilities, and if
so, which ones, to whom and when.

One model that is specifically enabled by this proposal, but is not
required or even recommended, is a separation of the roles of the
IETF Chair from that of the IESG Chair, allowing another Area
Director to take over the chairperson role of the IESG and its
associated responsibilities. It also enables delegation of the IETF
Chair's full IAB membership, and delegation or sharing of the role of
General Area Director.

# Separating the IETF Chair and IESG Chair Roles

This section analyzes which RFCs imply that the IETF Chair and IESG
Chair roles need to be filled by the same person, and makes
suggestions for updates that would allow a separation.

## Background

{{!RFC2026}} is surprisingly silent on the role of the IETF Chair,
only mentioning it in {{Section 14 of !RFC2026}} as part of the
terminology:

> Area Director - The manager of an IETF Area.  The Area Directors
  along with the IETF Chair comprise the Internet Engineering
  Steering Group (IESG).

> Internet Engineering Steering Group (IESG) - A group comprised of
  the IETF Area Directors and the IETF Chair. (...)

Similarly, the role of the IESG Chair is only briefly mentioned in
{{Section 6.5.2 of !RFC2026}} as part of how process failures are
handled:

> If an individual should disagree with an action taken by the IESG in
  this process, that person should first discuss the issue with the
  IESG Chair. If the IESG Chair is unable to satisfy the complainant
  then (...)

{{!RFC2026}} does not require the IETF Chair to also fulfill the role
of IESG Chair. {{Section 1.2 of ?RFC1602}}, the earlier revision of
the standards process that {{!RFC2026}} obsoletes, is an
Informational RFC and does include text to that effect, however:

> The IESG is composed of the IETF Area Directors and the
  chairperson of the IETF, who also serves as the chairperson of the
  IESG.

{{Section 1.2 of ?RFC1602}} is likely the basis for
{{?RFC2028}}, a BCP that includes similar text:

> The IESG is composed of the IETF Area Directors and the chair of the
  IETF, who also serves as the chair of the IESG.

{{Section 3.3 of !RFC9281}}, a BCP that obsoletes
{{?RFC2028}}, retains that text and also states that the IETF Chair is
the Area Director for the General Area:

> The IESG is composed of the ADs and the IETF Chair. The IETF Chair
  also chairs the IESG and is the AD for the General Area.

{{Section 4 of !RFC4949}}, an Informational RFC containing an Internet
Security Glossary, contains this text under the "Internet Engineering
Steering Group (IESG)" glossary item:

> The part of the ISOC responsible for technical management of IETF
  activities and administration of the Internet Standards Process
  according to procedures approved by the ISOC Trustees. Directly
  responsible for actions along the "standards track", including
  final approval of specifications as Internet Standards. Composed of
  IETF Area Directors and the IETF chairperson, who also chairs the
  IESG. (RFC 2026)

## Proposal {#prop-chair-roles}

In order to allow the IETF Chair to delegate the role of IESG Chair to
another AD (as arguably intended to be allowed by {{!RFC2026}}), the
following updates to existing RFCs are proposed:

1. Remove the sentence "The IETF Chair also chairs the IESG and is the
AD for the General Area." from {{Section 3.3 of !RFC9281}}.

1. Remove the clause "who is also the chair of the Internet
Engineering Steering Group (IESG)", from the second sentence of
{{Section 1 of !RFC2850}}. (This is also part of the suggestions in
{{prop-gen-ad}}.)

1. Remove the clause "who also chairs the IESG" from the "Internet
Engineering Steering Group (IESG)" glossary item in {{Section 4
of !RFC4949}}.

# Allowing the IETF Chair to Delegate their IAB Membership

This section analyzes which RFCs contain text about the full IAB
membership of the IETF Chair, and makes suggestions for updates that
would allow delegation of the IAB membership.

## Background

{{Section 1 of !RFC2850}} requires the IETF Chair to be a full member
if the IAB:

> The Internet Architecture Board (IAB) shall consist of thirteen full
  members, composed of the chair of the Internet Engineering Task
  Force (IETF), and of twelve sitting members.

{{Appendix C of !RFC8713}} contains a similar statement as part of as
the second item in a list of "oral traditions" recorded
for "consideration by future NomComs":

> No person should serve both on the IAB and as an Area Director,
  except the IETF Chair whose roles as an IAB member and Area
  Director of the General Area are set out elsewhere.

{{Section 3.4 of !RFC9281}} says:

> The IETF Chair is also a member of the IAB, and the Chair of the
  Internet Research Task Force (IRTF) is an ex officio member.

## Proposal

In order to allow the IETF Chair to delegate their full IAB membership
to another AD, the following updates to existing RFCs are suggested:

1. Add "or their Delegate Area Director" at the end of the
clause "composed of the chair of the Internet Engineering Task Force
(IETF)" in {{Section 1 of !RFC2850}}.

1. Add "With the publication of RFCXXXX, IETF guidance on this issue
has changed as described there." to the second bullet item in
{{Appendix C of !RFC8713}}.

1. Change the sentence "The IETF Chair is also a member of the IAB,
and the Chair of the Internet Research Task Force (IRTF) is an ex
officio member." to "The Chair of the Internet Research Task Force
(IRTF) is an ex officio member of the IAB." in {{Section 3.4
of !RFC9281}}.

# Allowing the IETF Chair to Delegate their General Area Director Role

This section analyzes which RFCs contain text about the responsibility
of the IETF Chair to also serve as Area Director of the General Area,
and makes suggestions for updates that would allow delegation of or
sharing or the role.

## Background

{{Section 2 of !RFC3710}} states that the IETF Chair is the General
Area Director:

> The IETF Chair, who also functions as the General Area Director when
  this area is active

{{Section 3.3 of !RFC9281}} also makes a similar statement:

> The IETF Chair also chairs the IESG and is the AD for the General
  Area.

## Proposal {#prop-gen-ad}

In order to allow the IETF Chair to delegate the Area Director rols
for the General Area, the following updates  to existing RFCs are
suggested:

1. Replace "who also functions as the General Area Director" with "who
may also function as a General Area Director or may share that role
with or delegate that role to another Area Director" in {{Section 2
of !RFC3710}}.

1. Remove the clause "who is also the chair of the Internet
Engineering Steering Group (IESG)", from the second sentence of
{{Section 1 of !RFC2850}}. (This is also part of the suggestions in
{{prop-chair-roles}}.)

# Other Updates

This section collects updates to some text in existing RFCs that has
become stale.

## Staff Supervision

{{Section 7.1 of !RFC3710}} says

> The IETF Chair has primary responsibility for supervising the work
  of the IETF Secretariat, with the advice and consent of the IESG,
  the IAB Chair and the ISOC president.

With the publication of {{?RFC8711}}, this responsibility has moved to
the IETF Executive Director. The proposal is to update
{{Section 7.1 of !RFC3710}} to remove the sentence above.

# Other Roles

This section briefly summarizes other roles the IETF Chair has, but
which require no updates, usually because delegation is already
permitted.

## Liaison Statements

{{Section 3.1 of ?RFC4691}} says

> Liaison statements are only sent on the initiative of the IETF
  chair, the IAB chair, IETF Area Directors, or IETF working group
  chairs.

{{Section 4 of ?RFC4052}} says

> For a liaison statement generated on behalf of the IETF as a whole,
  the IETF Chair must have generated or must agree with the sending
  of the liaison statement.  If the liaison statement is not sent by
  the IETF Chair, then his or her agreement must be obtained in
  advance and confirmed by copying the IETF Chair on the message.

The combination of these two statements already allows another Area
Director to send a liaison statement on behalf of the IETF with IETF
Chair approval.

## Transgressions of the IETF Guidelines for Conduct

{{Appendix A of ?RFC7154}} says "An individual can report
transgressions of the guidelines for conduct to the IETF Chair or the
IESG."

However, {{?RFC7154}} does not define any reactions the IETF Chair or
the IESG should or may take, so the IETF Chair only acts as a
recipient here.

## Managing the Ombuds- and Moderator Teams

The IETF Chair is tasked with managing the constituency of the
ombudsteam {{?RFC7776}} and the moderator team of the IETF discussion
list {{?RFC9245}}.

This document does not suggest any changes here, but the community may
consider allowing delegation of either of these responsibilities if
revisions of {{?RFC7776}} or {{?RFC9245}} are undertaken.

## Serving on the IETF LLC Board

{{?RFC8711}} suggests that the IETF Chair, or a delegate selected by
the IESG, will serve on the Board of Directors of the IETF
Administration LLC. Because delegation of that role is already
explicitly allowed, no changes are suggested here.

Done:

- {{!RFC2026}} says

  - "IETF Chair is part of the IESG" N/A

  - "If the IESG Chair is unable to satisfy the complainant" only
     mention of IESG chair?
  - no mention of IETF Chair being IESG Chair (but the obsolete
    {{?RFC1602}} said that)

- {{!RFC2418}} only says "IETF Chair is part of the IESG" N/A

- {{!RFC4949}} says "IETF chairperson, who also chairs the IESG"

- {{!RFC8713}} says "No person should serve both on the IAB and as an
  Area Director, except the IETF Chair whose roles as an IAB member
  and Area Director of the General Area are set out elsewhere." N/A

- {{!RFC2850}} says

  - "the IETF Chair is on the IAB" and that each body appoints another
     liaison (not the IETF Chair) to each other - delegation
     implied?

  - "The IETF chair, who is also the chair of the Internet Engineering
     Steering Group (IESG)"

- {{!RFC9281}} says
  - "The IESG is composed of the ADs and the IETF Chair. The IETF
     Chair also chairs the IESG and is the AD for the General Area."
     First mention of IESG chair?
  - "The IETF Chair is also a member of the IAB"

- {{!RFC3710}} says

  - "IETF Chair is *the* GEN AD"

  - "The IETF Chair has primary responsibility for supervising the
     work of the IETF Secretariat, with the advice and consent of the
     IESG, the IAB Chair and the ISOC president." Outdated?

- {{?RFC7776}}
  - "The Ombudsteam is appointed by the IETF Chair." Also
     reappointment, removal, etc.

  - "In determining the appropriate training, the IETF Chair and
     Ombudsteam shall take professional advice"

  - "The IETF will, however, meet the costs of training when agreed to
     by the IETF Chair"

  - "3.8.  Disputes with the IETF Chair Regarding the Ombudsteam" all
     with the Chair

  - "IETF Chair may recuse themself from any part of this process
     (see Section 7) and request the IESG to select another of its
     members to serve in this role" all dispute resolution

- {{!RFC9245}} all moderator management


N/A

- {{!RFC8711}} says

  - "Board Composition: 1 IETF Chair or delegate selected by the IESG"

  - "presumption is that the IETF Chair will serve on the board"

- {{!RFC8716}} just updates 7776 w N/A

- {{!RFC8719}} says "timing and frequency of future exploratory
  meetings will be based on IETF consensus as determined by the IETF
  chair" Mostly done by exec dir, but consensus confirmed by chair.

- {{!RFC4053}} says "incoming LS are CC'ed to the IETF Chair if they
  go to an AD"



- {{!RFC7704}} says "Depending on the details, the working group
  chair, mailing list moderator, Ombudsperson, or perhaps IETF Chair
  is the appropriate person to contact." Why not AD?

# Security Considerations

TODO Security

# IANA Considerations

This document has no IANA actions.

# Acknowledgments
{:numbered="false"}

TODO acknowledge.

--- back

# Changing the Status of Some RFCs to "Historic"

When researching RFCs that mention the IETF Chair or the IESG Chair, a
number of RFCs were identified that should be move to "Historic"
status via a "status change" IESG action:

- {{?RFC1052}}
- {{?RFC1118}}
- {{?RFC1120}}
- {{?RFC1160}}
- {{?RFC1177}}
- {{?RFC1206}}
- {{?RFC1287}}
- {{?RFC1310}}
- {{?RFC1325}}
- {{?RFC1358}}
- {{?RFC1371}}
- {{?RFC1380}}
- {{?RFC1391}}
- {{?RFC1396}}
- {{?RFC1506}}
- {{?RFC1539}}
- {{?RFC1601}}
- {{?RFC1602}}
- {{?RFC1603}}
- {{?RFC1640}}
- {{?RFC1719}}
- {{?RFC1752}}
- {{?RFC2028}}
- {{?RFC2057}}
- {{?RFC2828}}
- {{?RFC3005}}
- {{?RFC3716}}
- {{?RFC3777}}
- {{?RFC3844}}
- {{?RFC4071}}
- {{?RFC4089}}
- {{?RFC4333}}
- {{?RFC4441}}
- {{?RFC4633}}
- {{?RFC7437}}
- {{?RFC7500}}
- {{?RFC7749}}
- {{?RFC7979}}
- {{?RFC8318}}

# Mentioning, but no change proposed

- {?RFC2804}
- {?RFC2860}
- {?RFC3714}
- {?RFC3869}
- {?RFC4440}
- {?RFC6335}
- {?RFC6462}
- {?RFC6641}
- {?RFC6702}
- {?RFC6717}
- {?RFC6733}
- {?RFC6764}
- {?RFC6852}
- {?RFC6921}
- {?RFC6940}
- {?RFC7252}
- {?RFC7319}
- {?RFC7322}
- {?RFC7350}
- {?RFC7360}
- {?RFC7510}
- {?RFC7585}
- {?RFC7589}
- {?RFC7624}
- {?RFC7669}
- {?RFC7687}
- {?RFC7808}
- {?RFC7858}
- {?RFC7881}
- {?RFC8030}
- {?RFC8071}
- {?RFC8086}
- {?RFC8314}
- {?RFC8323}
- {?RFC8462}
- {?RFC8545}
- {?RFC8572}
- {?RFC8620}
- {?RFC8715}
- {?RFC8782}
- {?RFC8803}
- {?RFC8915}
- {?RFC8926}
- {?RFC8968}
- {?RFC8973}
- {?RFC8990}
- {?RFC9132}
- {?RFC9250}
- {?RFC9393}
