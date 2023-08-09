---
title: "The IETF Chair May Delegate"
# abbrev: ""
category: bcp

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
responsibilities to other individuals.

--- middle

# Introduction

Throughout the history of the IETF, the role of the IETF Chair has
always been a filled by a single person. None of the foundational
documents of the organization precisely define the role, but most are
written with an understanding that the role is filled by a single
person that is then tasked with with numerous responsibilities. Few
documents explicitly say that the IETF Chair may delegate some of
these responsibilities.

Single bottlenecks like this have obvious scaling and fault tolerance
issues. This document hence proposes to explicitly allow the IETF
Chair to delegate some of their responsibilities to other
individuals, specifically, other Area Directors. It leaves it up to
each IETF Chair to determine if they would like to delegate some of
their responsibilities, and if so, which ones and when.

# Motivation

Over time, numerous RFCs have added responsibilities for the IETF
Chair in a piecemeal fashion, to a point where even a full-time
committment by a single person may no longer be sufficient to fulfill
all of them.

Additionally, the role of the IETF Chair is a single point of failure
for the organization, with no defined processes for allowing others
to quickly and/or temporarily take over aspects of the role if the
IETF Chair becomes partially or fully unable to serve. (The defined
process is that for "mid-term vacancies" per {{Section 3.5
of !RFC8713}}, which can take up to six weeks to complete and only
allows for the permanent replacement of the IETF Chair by another
individual.)

# RFCs Mentioning the IETF Chair

Work require:

- {{!RFC2026}} says
  - "IETF Chair is part of the IESG" N/A
  - "If the IESG Chair is unable to satisfy the complainant" only
     mention of IESG chair?
- {{!RFC2418}} only says "IETF Chair is part of the IESG" N/A
- {{!RFC2850}} says "the IETF Chair is on the IAB" and that each body
  appoints another liaison (not the IETF Chair) to each other -
  delegation implied?
- {{!RFC3710}} says
  - "IETF Chair is *the* GEN AD"
  - "The IETF Chair has primary responsibility for supervising the
     work of the IETF Secretariat, with the advice and consent of the
     IESG, the IAB Chair and the ISOC president." Outdated?
- {{!RFC4052}} says "For a liaison statement generated on behalf of
  the IETF as a whole, the IETF Chair must have generated or must
  agree with the sending of the liaison statement..."
- {{!RFC4053}} says "incoming LS are CC'ed to the IETF Chair if they
  go to an AD"
- {{!RFC4691}} says "Liaison statements are only sent on the
  initiative of the IETF chair, the IAB chair, IETF Area Directors,
  or IETF working group chairs." Already OK if delegate is AD.
- {{!RFC7154}} says "An individual can report transgressions of the
  guidelines for conduct to the IETF Chair or the IESG." Already OK
  if delegate is AD.
- {{!RFC7704}} says "Depending on the details, the working group
  chair, mailing list moderator, Ombudsperson, or perhaps IETF Chair
  is the appropriate person to contact." Why not AD?
- {{!RFC7776}} says
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
- {{!RFC8711}} says
  - "Board Composition: 1 IETF Chair or delegate selected by the IESG"
  - "presumption is that the IETF Chair will serve on the board"
- {{!RFC8713}} says "No person should serve both on the IAB and as an
  Area Director, except the IETF Chair whose roles as an IAB member
  and Area Director of the General Area are set out elsewhere." N/A
- {{!RFC8716}} just updates 7776 w N/A
- {{!RFC8719}} says "timing and frequency of future exploratory
  meetings will be based on IETF consensus as determined by the IETF
  chair" Outdated, done by exec dir.
- {{!RFC9245}} all moderator management
- {{!RFC9281}} says
  - "The IESG is composed of the ADs and the IETF Chair. The IETF
     Chair also chairs the IESG and is the AD for the General Area."
     First mention of IESG chair?
  - "The IETF Chair is also a member of the IAB"


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
- {{?RFC4949}}
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
