# Security Incident Response Plan for Identity Python-governed Projects

## Version 0.5 2021-02-02

_Approved by the idpy Board on 18 March 2021_

The following details the steps and actions that we should consider when
responding to security issues related to projects governed by the Identity
Python project. Some steps may not be necessary in all cases. Regardless, the
Identity Python members should follow a _no-blame policy_; the focus should
always be on improving the project rather than pointing fingers at
contributors.

Recognizing the importance of security research
we will publicly acknowledge the people that report an incident, granted their consent,
on a dedicated page on [the Identity Python website][idpyweb].

| Stage | Activities |
| ----- | ---------- |
| Discovery and Assignment | Reporter: <ul> <li>Anyone can submit a potential security vulnerability to <incident-response@idpy.org> </li></ul>Project Architect:<ul><li>Creates security advisory in GitHub; this automatically assigns a Common Vulnerabilities and Exposures Identifier (CVE-ID).</li><li>Sends an email regarding the potential issue to the Board.</li><li>Acknowledges reporter.</li></ul> |
| Assessment and Remediation | Project Architect:<ul><li>Validates – confirms a vulnerability exists and creates a test for it</li><li>Classifies - Severity/Impact of the vulnerability is determined using Common Vulnerability Scoring System ([CVSS]). Specific potential impact to application is noted (e.g., Exploit allows Admin level access to application).</li><li>Identifies affected products/versions - Identifies all versions affected by the vulnerability and makes a note in the issue.</li><li>Briefs the reporter on the assessment as appropriate.</li><li>Works with other technical resources in the community on the remediation.</li><li>Identifies remediation options and determine best remediation strategy as a result of the analysis.</li><li>Implements a fix for issue in a the appropriate project repo.</li><li>Validates that the issue is resolved. Ideally this involves a second organization.</li><li>Creates a test to verify the issue does not come up again in future versions.</li></ul>|
| Community Disclosure and Patch Release | Project Architect:<ul><li>Announces vulnerability and release date.</li><li>Creates patch release or remediation instructions.</li><li>Publishes patch release in consultation with the Incident Manager.</li><li>Sends disclosure notice to code repository owners.</li></ul> |
| Post-Mortem Retrospective | <ul><li>The Board discusses the Security Incident Response Plan as it played out for this incident, inspecting and adapting to handle the next one better.</li><li>The <discuss@idpy.org> list discusses the technical substance of the vulnerability and its fix, identifying opportunities to refactor the fix in subsequent releases now that it has more eyes on it and opportunities to improve the product and development practices to prevent or mitigate similar issues in the future.</li></ul> |

## Storage policy for incident reports

Incident reports are stored for the duration of the Identity Python project
in the form of mailing list archives on the <incident-response@idpy.org> mailing list,
and in the list of GitHub issues filled under the appropriate project-repository.

# Appendix A: Templates

## Reporter acknowledgement

```
To: <reporter>
Cc: incident-response@idpy.org
Subject: Security vulnerability acknowledgement

This is an acknowledgement of your email. Thank you for reporting this. We will
take this under advisement and address as appropriate. You can expect the
incident manager to reach out to you in the near future. For more information,
see the idpy Security Incident Response Plan (<link>).

Sincerely,
<security-monitor>
```

## Private disclosure

```
To: <technical-resource>
Subject: Private notice of critical security vulnerability in <product>

This is a private disclosure of a critical security vulnerability that has been
discovered in <product>. Affected versions are susceptible to an open redirect
vulnerability in the ....

Affected Software: <product>
Vulnerable versions: <x.y.z>
Fix version: <x.y.z'>

Impact:
<description>

Remediation:
Upgrade affected <product> deployments as soon as possible using the link above.
```

## Public disclosure

```
To: incident-response@idpy.org, discuss@idpy.org, satosa-dev@lists.sunet.se
Subject: Notice of critical security vulnerability in <product>

This is a public disclosure of a critical security vulnerability that has been
discovered in <product>. Affected versions are susceptible to an open redirect
vulnerability in the ....

Affected Software: <product>
Vulnerable versions: <x.y.z>
Fix version: <x.y.z'>

Impact:
<description>

Remediation:
Upgrade affected <product> deployments as soon as possible using the link above.
```

---

  [idpyweb]: https://idpy.org
  [CVE-ID]: http://iwantacve.org/
  [CVSS]: http://nvd.nist.gov/cvss.cfm
