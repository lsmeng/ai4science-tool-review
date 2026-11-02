# AI for Science tool review (pilot)

An informal, community-run review for Claude skills and connectors, run as a one-month pilot by members of the AI for Science community (9 November to 9 December 2026). Discussion and announcements are on the AI for Science Discourse. This is a community experiment, not an official Anthropic review or certification.

## Why

Anyone can share a skill or connector on GitHub, but a scientist from outside a subfield can not easily tell whether it installs and reproduces known results. Here a volunteer reviewer from the field runs a specific version of the tool on one or two cases with known answers and posts a short report. If the cases are reproduced, the submission gets a `tested` label with a link to the report. The label means one reviewer reproduced those cases on that version, it is not a guarantee of general correctness.

## Submitting a tool

Open a new issue with the **Tool submission** template. You will be asked for a link to the tool and the version or commit, the authors, what it needs to run, a short description, the field, and one or two test cases with known answers that a reviewer can start from. You can submit tools you wrote or tools from your group. Test cases should use open data and free endpoints, so a reviewer does not need paid credentials.

## Reviewing

Sign up with the reviewer form (link on the Discourse post). You choose your subfields and how many reviews you are willing to do during the pilot. Submissions are assigned in turn. When you get one, please reply on the issue within 3 days to accept or pass, and post your report as a comment on the issue within about a week, using the [review report template](REVIEW_TEMPLATE.md). Most reviews should take about half a day.

AI agents may run the same tools in the background, and reviewer reports may be compared with their results, to learn how far automated testing can be trusted. This comparison does not affect the label of a tool during the pilot.

A review is not a peer review of a paper. The questions are simple: does it install, does it reproduce the known cases, and what are its limits.

Reviewers and area editors do not handle tools from their own group or close collaborators. When an area editor submits a tool, another area editor or an independent volunteer handles that issue.

Skills and connectors run code on your machine. Please look through the repository before installing, and run unfamiliar tools in a container, a VM or a restricted account without sensitive keys. If a submission needs paid credentials, proprietary software or hardware you do not have, please pass on it.

## Outcomes

- `tested`: the cases were reproduced on the reviewed version
- `tested-with-caveats`: reproduced, with notable limitations
- `needs-changes`: installation failed or the cases did not match

After `needs-changes` the author may push fixes and post the new commit on the same issue, for a brief re-check by the reviewer (if willing) or the area editor. A label applies only to the version that was reviewed.

## Recognition

Reviewers and the tools they reviewed are listed on the Discourse at the end of the pilot.

## Fields and area editors

| Field | Area editor |
|---|---|
| Earth science | Lingsen Meng (UCLA) |
| Other fields | open, please volunteer on the Discourse |

Area editors step in when a submission is not picked up or when author and reviewer disagree.

## Labels

- `submission`: added automatically when a tool issue is opened
- `field:<name>`: routes the submission, e.g. `field:earth-science`
- `assigned`, `in-review`, plus the three outcomes above

## License

Review reports are published under CC BY 4.0. All other material in this repository is copyright Lingsen Meng, all rights reserved. See [LICENSE](LICENSE).
