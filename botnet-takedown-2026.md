# How 3 Million Ordinary Devices Became the Most Dangerous Weapons on the Internet

---

## Overview

In March 2026, the U.S. Department of Justice, alongside international law enforcement
partners in Canada and Germany, executed one of the most significant botnet disruption
operations in recent history. The coordinated action targeted four highly destructive
botnet networks responsible for hundreds of thousands of cyberattacks worldwide,
affecting millions of devices and costing victims tens of thousands of dollars in
damages and remediation costs.

This article breaks down what happened, how these botnets operated, and what it means
for individuals and organizations navigating today's threat landscape. This story matters
because awareness matters. Understanding what these threats are and how they work is your
first line of defense. At Verdilock Cybersecurity, our mission is to decode the latest
cyber threats so that individuals and organizations stay one step ahead and this operation
is exactly the kind of story our community needs to understand.

---

## The Four Botnets

The operation targeted four distinct botnet networks, each with its own infrastructure,
scale, and attack methodology.

### Aisuru

Aisuru emerged in late 2024 and rapidly became one of the most active and destructive
botnets ever recorded. It primarily targeted networking equipment including routers, IP
cameras, and Wi-Fi gateways. By mid-2025, it was responsible for record-breaking
Distributed Denial of Service (DDoS) attacks, including a confirmed attack against
Microsoft Azure. Aisuru issued more than **200,000 DDoS attack commands** throughout its
operation. The speed at which Aisuru grew from emergence to record-breaking attacks in
under a year is a sobering reminder of how rapidly the threat landscape can shift and how
quickly organizations must adapt their defenses.

### Kimwolf

Kimwolf was a successor variant of Aisuru, introduced in October 2025 with a novel and
particularly dangerous spreading mechanism. Unlike traditional botnets that scan the open
internet for vulnerable devices, Kimwolf exploited residential proxy networks to infiltrate
devices that were protected behind home and corporate firewalls. It primarily targeted
Android-based streaming devices, smart TVs, and set-top boxes, growing to over
**1.8 million infected devices**. It issued more than **25,000 DDoS attack commands**.
What makes Kimwolf particularly significant is that the very networks designed to protect
devices became the attack vector, a technique that fundamentally challenges how we think
about perimeter security.

### JackSkid

JackSkid adopted the same residential proxy exploitation technique as Kimwolf, allowing
it to compromise devices that were never meant to be publicly accessible. In the days
leading up to the takedown, JackSkid was averaging over **150,000 daily victims**,
peaking at 250,000 on March 8, 2026. It launched more than **90,000 DDoS attack
commands**. Of the four botnets in this operation, JackSkid stood out the most to me.
Not because it was the largest, but because of what those numbers represent in human
terms. 150,000 daily victims means 150,000 individuals and organizations every single day
whose devices were being used as weapons against others while they had absolutely no idea
it was happening. That is not a statistic. That is a reality check.

### Mossad

Mossad was the smallest of the four botnets but still averaged over **100,000 daily
victims** in early March 2026. It launched more than **1,000 DDoS attack commands** and
exploited the same Android Debug Bridge vulnerability leveraged by Kimwolf and JackSkid.
Mossad is a reminder that in cybersecurity, smaller does not mean less dangerous. 100,000
daily victims is not a minor operation by any measure and even secondary threat actors in
an operation of this scale can cause significant and lasting harm.

---

## The Scale of the Threat

To understand the severity of these attacks, consider the following:

- The four botnets collectively compromised **more than 3 million IoT devices** worldwide,
  with hundreds of thousands located inside the United States.
- At their peak, combined attack traffic reached **31.4 terabits per second**, a
  record-breaking figure. For context, this is the equivalent of the entire populations
  of the United Kingdom, Germany, and Spain all simultaneously loading a webpage at the
  exact same second.
- Across all four botnets, a combined total of more than **316,000 DDoS attack commands**
  were issued.
- Total DDoS attacks globally more than **doubled in 2025 to 47.1 million**, with
  network-layer attacks tripling year over year.

These were not fringe operations. They targeted critical infrastructure including
telecommunications companies, financial services organizations, and internet addresses
owned by the U.S. Department of Defense Information Network (DoDIN).

---

## How the Botnets Operated

To truly understand why this operation matters, it helps to look at exactly how these
botnets built their criminal infrastructure and why they were so difficult to detect
and dismantle.

**Device Infection**
Operators identified and exploited vulnerabilities in consumer-grade IoT devices,
including digital video recorders, webcams, routers, and Android smart TVs. Many of
these devices had unpatched firmware or exposed network interfaces, making them easy
targets.

**Command and Control (C2) Infrastructure**
Once infected, devices were folded into a centralized command and control network.
Operators issued instructions remotely through C2 servers, directing thousands of devices
simultaneously to flood targets with traffic.

**Cybercrime as a Service**
Access to the botnets was sold on criminal forums to third parties. Customers could rent
the infrastructure to launch DDoS attacks against targets of their choosing or use
infected devices as anonymous proxies to mask other criminal activity. In some cases,
operators directly extorted victims, demanding payment to stop ongoing attacks.

---

## The Takedown Operation

The disruption was a court-authorized, multi-agency operation executed simultaneously
across three countries.

The U.S. Defense Criminal Investigative Service (DCIS) executed seizure warrants
targeting U.S.-registered domains, virtual servers, and other C2 infrastructure. In
parallel, law enforcement in Canada and Germany conducted actions against individuals
believed to operate the botnets.

Nearly two dozen major technology companies assisted in the investigation and operation,
including Akamai, Amazon Web Services, Cloudflare, DigitalOcean, Google, Lumen, Nokia,
Okta, Oracle, and PayPal. Lumen's security research team alone null-routed nearly 1,000
C2 servers linked to Aisuru and Kimwolf.

---

## What This Means Going Forward

While the operation successfully dismantled the command and control infrastructure of all
four botnets, it is important to understand what the takedown did and did not accomplish.

**What was achieved:**
- Seizure of domains and servers used to coordinate attacks
- Disruption of the botnets' ability to issue new attack commands
- Prevention of further device infections through those specific networks

**What remains a concern:**
- Millions of previously infected devices remain compromised and vulnerable unless their
  owners apply firmware updates or replace the devices entirely. The infrastructure is
  gone but the infected devices are still out there, still vulnerable, and still waiting
  to be recruited into the next criminal network. This is perhaps the most critical detail
  that most headlines missed entirely.
- The underlying malware code was not eliminated and copycat networks have already begun
  emerging. In cybersecurity, taking down a botnet often feels like cutting off one head
  of a hydra. The code survives, the techniques are documented, and new operators are
  always ready to rebuild using the same blueprint.
- The residential proxy exploitation technique pioneered by Kimwolf and JackSkid has been
  adopted by other threat actors.

---

## Key Takeaways for Individuals and Organizations

1. **Every device connected to your network is a potential entry point.** Routers,
   webcams, smart TVs, and DVRs are not passive tools. If left unpatched and unmonitored
   they can be silently recruited into criminal networks without you ever knowing.

2. **Firmware updates are not optional.** The majority of infected devices in this
   operation were running outdated software with known vulnerabilities. Regular updates
   are one of the most effective and accessible defenses available to anyone.

3. **Network visibility matters.** Organizations should maintain awareness of every device
   connected to their network. An unmanaged IoT device is a potential entry point for
   threat actors.

4. **DDoS is not just a large organization problem.** Small and mid-sized businesses are
   increasingly targeted because they often lack the mitigation infrastructure of larger
   enterprises.

5. **Awareness is the foundation of every strong security posture.** The biggest gap in
   cybersecurity is not always technology. It is understanding. Most people do not know
   what a botnet is until one is quietly using their device against someone else. Closing
   that knowledge gap is exactly why Verdilock Cybersecurity exists.

---

## Conclusion

The dismantling of Aisuru, Kimwolf, JackSkid, and Mossad represents a meaningful victory
for international law enforcement and the cybersecurity community. However, it also serves
as a clear reminder that the threat landscape continues to evolve in scale and
sophistication. As botnets grow larger, faster, and more difficult to detect, staying
informed is no longer optional. It is essential. At Verdilock Cybersecurity, our
commitment is to make sure that the next time a story like this breaks, our community
already understands what it means, why it matters, and what to do about it.

---

**Author:** Daphne Daguia, MS-CYB
**Published:** © April 2026 Verdilock Cybersecurity. All rights reserved.
