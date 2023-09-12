---
title: "The IETF Chair May Delegate"
category: bcp
updates: 2850, 3710, 4949, 8713, 9281
docname: draft-eggert-ietf-chair-may-delegate-latest
submissiontype: IETF
consensus: true
v: 3
workgroup: "IETF"
venue:
  group: "IETF"
  type: "Internet Engineering Task Force"
  mail: ""
  arch: ""
  github: "larseggert/ietf-chair-may-delegate"
  latest: "https://larseggert.github.io/ietf-chair-may-delegate/draft-eggert-ietf-chair-may-delegate.html"

author:
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

This document proposes that the IETF Chair may delegate some of their
responsibilities to other Area Directors, and updates several
existing RFCs to enable that. It also proposes a succession of
emergency stand-ins in case the IETF Chair becomes incapacitated.

--- middle

# Introduction {#intro}

Throughout the history of the IETF, the role of the IETF Chair has
always been filled by a single person. None of the foundational
documents of the organization precisely define the role, but most are
written with an understanding that the role is filled by a single
person who is then tasked with numerous responsibilities. The expired
Internet-Draft {{?I-D.carpenter-ietf-chair-tasks}} attempted to
define the role of the IETF Chair more precisely but was not taken
forward.

Few documents explicitly say that the IETF Chair may delegate some of
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
Chair's full IAB membership and delegation or sharing of the role of
the General Area Director.

Specifically, with these changes, it should be possible for the IESG
to request the selection of a General Area Director who is not at the
same time also the IETF Chair, to whom the IETF Chair may then
delegate some of their responsibilities, such as chairing the IESG.

There must be community transparency about which roles the IETF Chair
has delegated to which other Area Director, and for which time. This
transparency can be guaranteed in several ways, such as through the
IESG website or public email. Such operational details are out of the
scope of this document.

# Emergency Stand-In

This section describes who may stand in for the IETF Chair in case of
emergency if they become unable to fulfill their duties.

## Background

As described in {{intro}}, the IETF Chair role is at the moment a
single point of failure for the organization. In an emergency that
incapacitated the IETF Chair, a recall petition followed by executing
a "mid-term vacancy" replacement would need to be executed to name a
new IETF Chair. This process will likely take several weeks at best,
during which time there is no defined stand-in for the IETF Chair.

## Proposal

This document proposes that in the case the IETF Chair becomes
incapacitated, the IAB Chair will automatically assume the role of
the IETF Chair. If the IAB Chair is unable to do so, the IETF Chair
role will automatically fall to the Chair of the IETF Administration
LLC. As soon as the NomCom appoints a new IETF Chair this emergency
delegation ends.

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
>
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

To allow the IETF Chair to delegate the role of IESG Chair to another
AD (as arguably intended to be allowed by {{!RFC2026}}), the
following updates to existing RFCs are proposed:

1. Remove the sentence "The IETF Chair also chairs the IESG and is the
AD for the General Area." from {{Section 3.3 of !RFC9281}}.

1. Change the clause "The IETF chair, who is also the chair of the
Internet Engineering Steering Group (IESG)" in the second sentence
of {{Section 1 of !RFC2850}} to "The IETF chair or their delegate".
(This is also part of the suggestions in {{prop-gen-ad}}.)

1. Remove the clause "who also chairs the IESG" from the "Internet
Engineering Steering Group (IESG)" glossary item in {{Section 4
of !RFC4949}}.

# Delegation of the IAB Membership

This section analyzes which RFCs contain text about the full IAB
membership of the IETF Chair, and makes suggestions for updates that
would allow delegation of the IAB membership.

## Background

{{Section 1 of !RFC2850}} requires the IETF Chair to be a full member
of the IAB:

> The Internet Architecture Board (IAB) shall consist of thirteen full
  members, composed of the chair of the Internet Engineering Task
  Force (IETF), and of twelve sitting members.

{{Appendix C of !RFC8713}} contains a similar statement as part of the
second item in a list of "oral traditions" recorded
for "consideration by future NomComs":

> No person should serve both on the IAB and as an Area Director,
  except the IETF Chair whose roles as an IAB member and Area
  Director of the General Area are set out elsewhere.

{{Section 3.4 of !RFC9281}} says:

> The IETF Chair is also a member of the IAB, and the Chair of the
  Internet Research Task Force (IRTF) is an ex officio member.

## Proposal

To allow the IETF Chair to delegate their full IAB membership to
another AD, the following updates to existing RFCs are suggested:

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

# Delegation of the General Area Director Role

This section analyzes which RFCs contain text about the responsibility
of the IETF Chair to also serve as Area Director of the General Area,
and makes suggestions for updates that would allow delegation of or
sharing of the role.

## Background

{{Section 2 of !RFC3710}} states that the IETF Chair is the General
Area Director:

> The IETF Chair, who also functions as the General Area Director when
  this area is active

{{Section 3.3 of !RFC9281}} also makes a similar statement:

> The IETF Chair also chairs the IESG and is the AD for the General
  Area.

## Proposal {#prop-gen-ad}

To allow the IETF Chair to delegate the Area Director role of the
General Area, the following updates  to existing RFCs are suggested:

1. Replace "who also functions as the General Area Director" with "who
may also function as a General Area Director or may share that role
with or delegate that role to another Area Director" in {{Section 2
of !RFC3710}}.

1. Change the clause "The IETF chair, who is also the chair of the
Internet Engineering Steering Group (IESG)" in the second sentence
of {{Section 1 of !RFC2850}} to "The IETF chair or their delegate".
(This is also part of the suggestions in {{prop-chair-roles}}.)

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

# Security Considerations

The usual security considerations {{?RFC3552}} do not apply to this
document.

# IANA Considerations

This document has no IANA actions.

# Acknowledgments

These individuals suggested improvements to this document:

- Alvaro Retana
- Brian Carpenter
--- back
